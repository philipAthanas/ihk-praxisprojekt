<template>
  <div>
    <div v-if="isUserSignedIn">
      <div>
        <img v-show="this.profilePic" :src="this.profilePic" />
      </div>
      <HeroSection />
    </div>
    <div v-else id="google-signin-button"></div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      isUserSignedIn: false,
      profilePic: null,
    };
  },
  mounted() {
    setTimeout(() => {
      gapi.signin2.render("google-signin-button", {
        onsuccess: this.onSignIn,
      });
    });
  },
  methods: {
    onSignIn(user) {
      // console.log("invoking onSignin...");
      const profile = user.getBasicProfile();
      /* console.log("ID: " + profile.getId());
      console.log("Full Name: " + profile.getName());
      console.log("Given Name: " + profile.getGivenName());
      console.log("Family Name: " + profile.getFamilyName());
      console.log("Image URL: " + profile.getImageUrl());
      console.log("Email: " + profile.getEmail()); */

      // The ID token you need to pass to your backend:
      var id_token = user.getAuthResponse().id_token;
      // console.log("ID Token: " + id_token);

      if (profile.getEmail().includes("@integr8.com")) {
        this.isUserSignedIn = true;
        this.profilePic = profile.getImageUrl();
      } else {
        window.alert("Du musst bei Integr8 arbeiten");
      }
    },
  },
};
</script>

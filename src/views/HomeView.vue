<script setup>
const onSignIn = (user) => {
  var profile = user.getBasicProfile();
};
</script>

<template>
  <main>
    <div class="block">
      <h1>You can now Sign in to our platform</h1>
      <div class="g-signin2" data-onsuccess="onSignIn" @click="onSignIn">
        Sign in
      </div>
    </div>
  </main>
</template>

<style lang="scss">
main {
  min-height: 100vh;
  padding: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Poppins", sans-serif;
  h1 {
    text-align: center;
    font-size: 25px;
  }
}
</style>

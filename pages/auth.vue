<script>
  import { Authenticator } from "@aws-amplify/ui-vue";
</script>

<template>
  <div class="bg-gray-800">
    <authenticator>
      <template v-slot="{ user, signOut }">
        <h1>Hello {{ user.username }}!</h1>
        <button @click="signOut">Sign Out</button>
      </template>
    </authenticator>
  </div>
</template>




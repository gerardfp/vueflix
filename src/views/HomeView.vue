<template>
  <div v-if="$auth.isAuthenticated">
    <p>Welcome {{ $auth.email }}!</p>
    <router-link to="/logout">Logout</router-link>    
  </div>
  <div v-else>
    <p>Please login:</p>
    <router-link to="/login">Login</router-link>
    <router-link to="/register">Register</router-link>
  </div>
</template>
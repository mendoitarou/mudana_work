<template>
  <div>
    <NuxtRouteAnnouncer />
    <div class="main">
      無駄なWork
    </div>
    <div class="twitter_share_button">
      <Twitter_Share />
    </div>
    <div class="copyright">
      <small><NuxtLink to="https://home.mendoitarou.com/">mendoitarou_</NuxtLink></small>
    </div>
  </div>
</template>

<style>
  .main {
    font-size: xx-large;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  
  .copyright {
    position: absolute;
    right: 5px;
    bottom: 0px;
  }

  .twitter_share_button {
    position: absolute;
    left: 5px;
    bottom: 0px;
  }
</style>

<script setup lang="ts">
  useHead({
    title: '無駄なwork',
    meta: [
      { name: 'description', content: '無駄なwork' }
    ]
  })
</script>

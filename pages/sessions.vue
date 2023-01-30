<script setup>
const sessions = [
  '9c3097e8-9255-4fc7-bd24-658e3df94eb4',
  '03f3795e-7f6e-4dad-b4df-c35f84603eed',
  '89393708-6eaf-411c-85ba-8f28b61a9e54',
  'eb07cd52-6ed5-4f5a-8095-b440a41c4ca7',
  '5bdcb1d8-ed13-4f07-892c-7ce80e7e8b02',
].map((session)=>({
  url:`/sessions/${session}`,
  text: session
}))
</script>

<template>
  <div class="sessions">
    Sessions

    <ul>
      <li v-for="session in sessions">
        <nuxt-link :to="session.url">
          {{session.text}}
        </nuxt-link>
      </li>
    </ul>

    <nuxt-page />


  </div>
</template>
<style>
.sessions a{background:#333; color#fff;}
</style>

<script setup>
const route = useRoute()
const {id} = route.params
</script>

<template>
    <div>
      <div>
        Session ID: {{id}}
      </div>
      <nuxt-link to="/sessions">
         Back
      </nuxt-link>
    </div>
</template>

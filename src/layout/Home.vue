<template>
  <main class="home">
      <Basic/>
      <Status/>
  </main>
</template>

<script>
import Basic from '@/components/Basic';
import Status from '@/components/Status';
export default {
    name: 'Home',
    components:{
        Basic,
        Status,
    }
}
</script>

<style>

</style>
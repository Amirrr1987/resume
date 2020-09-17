<template>
  <main class="home">
      <Basic/>
      <Status/>
      <Education/>
  </main>
</template>

<script>
import Basic from '@/components/Basic';
import Status from '@/components/Status';
import Education from '@/components/Education';
export default {
    name: 'Home',
    components:{
        Basic,
        Status,
        Education,
    }
}
</script>

<style>

</style>
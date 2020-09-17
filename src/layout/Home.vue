<template>
  <main class="home">
      <Basic/>
      <Status/>
      <Education/>
      <Description/>
  </main>
</template>

<script>
import Basic from '@/components/Basic';
import Status from '@/components/Status';
import Education from '@/components/Education';
import Description from '@/components/Description';
export default {
    name: 'Home',
    components:{
        Basic,
        Status,
        Education,
        Description,
    }
}
</script>

<style>

</style>
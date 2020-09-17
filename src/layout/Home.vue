<template>
  <main class="home">
      <Basic/>
      <Status/>
      <Education/>
      <Links/>
      <Description/>
  </main>
</template>

<script>
import Basic       from '@/components/Basic';
import Status      from '@/components/Status';
import Education   from '@/components/Education';
import Links       from '@/components/Links';
import Description from '@/components/Description';
export default {
    name: 'Home',
    components:{
        Basic,
        Status,
        Education,
        Links,
        Description,
    }
}
</script>

<style>

</style>
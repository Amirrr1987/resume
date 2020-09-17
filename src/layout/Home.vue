<template>
  <main class="home">
      <Basic/>
      <Status/>
      <Education/>
      <Certificate/>
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
import Certificate from '@/components/Certificate';
export default {
    name: 'Home',
    components:{
        Basic,
        Status,
        Education,
        Links,
        Description,
        Certificate,
    }
}
</script>

<style>

</style>
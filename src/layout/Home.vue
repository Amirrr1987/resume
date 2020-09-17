<template>
  <main class="home">
      <Basic/>
      <Status/>
      <Education/>
      <Language/>
      <Skill/>
      <Project/>
      <Course/>
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
import Course      from '@/components/Course';
import Project     from '@/components/Project';
import Language    from '@/components/Language';
import Skill       from '@/components/Skill';
export default {
    name: 'Home',
    components:{
        Basic,
        Course,
        Status,
        Education,
        Language,
        Skill,
        Project,
        Certificate,
        Links,
        Description,
    }
}
</script>

<style>

</style>
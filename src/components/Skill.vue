<template>
  <section class="skill">
    <div class="skill__container">
      <h3 class="skill__title"><i class="icon icon--file-code"></i>{{title}} :</h3>
          <OS class="skill__table"/>
          <CSS class="skill__table"/>
          <CSSFramework class="skill__table"/>
          <JavaScript class="skill__table"/>
          <JavaScriptFramework class="skill__table"/>
          <Software class="skill__table"/>
          <BackEndLang class="skill__table"/>
          <Editor class="skill__table"/>
    </div>
    
  </section>
</template>

<script>
import OS from '@/components/OS';
import CSS from '@/components/CSS';
import CSSFramework from '@/components/CSSFramework';
import JavaScript from '@/components/JavaScript';
import JavaScriptFramework from '@/components/JavaScriptFramework';
import Software from '@/components/Software';
import Editor from '@/components/Editor';
import BackEndLang from '@/components/BackEndLang';
export default {
  name: "Skill",
  components:{
    OS,
    CSS,
    CSSFramework,
    JavaScript,
    JavaScriptFramework,
    Software,
    Editor,
    BackEndLang
  },
  data() {
    return {
      title: "مهارت ها",
      items: [
        { 
          title: "نام" ,
          body : "امیر",
        },
        { 
          title: "تاریخ تولد",
          body:  "1366" ,
        },
        { 
          title: "وضیعت تاهل",
          body:  "متاهل" ,
        },
        
        { 
          title: "وضعیت سربازی",
          body:  "اتمام خدمت" ,
        },
      ],
    };
  },
};
</script>
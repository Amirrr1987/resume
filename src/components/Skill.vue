<template>
  <section class="skill">
    <div class="skill__container">
      <h3 class="skill__title">{{title}} :</h3>
      <table class="skill__table table">
        <thead class="table__thead thead">
          <tr class="thead__row">
          </tr>
        </thead>
      </table>
      <OS class="skill__table"/>
      <OS class="skill__table"/>
      <OS class="skill__table"/>
    </div>
    
  </section>
</template>

<script>
import OS from '@/components/OS';
export default {
  name: "Skill",
  components:{
    OS,
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
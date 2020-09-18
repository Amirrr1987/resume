<template>
  <section class="project">
    <div class="project__container">
     <h3 class="project__title" colspan="4"><i class="icon icon--file-code"></i>{{title}} :</h3>
      <table class="project__table table">
          <tr class="table__row">
            <th class="table__col" v-for="(item,index) in items" :key="index">{{item.title}}</th>
          </tr>
          <tr class="table__row">
            <td class="table__col" v-for="(item,index) in items" :key="index">{{item.body}}</td>
          </tr>
      </table>
    </div>
  </section>
</template>

<script>
export default {
  name: "Project",
  data() {
    return {
      title: "پروژه ها",
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
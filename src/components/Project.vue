<template>
  <section class="project">
    <div class="project__container">
      <table class="project__table table">
        <thead class="table__thead thead">
          <tr class="thead__row">
            <th class="thead__col thead--title" colspan="4">{{title}} :</th>
          </tr>
          <tr class="thead__row">
            <th class="thead__col" v-for="(item,index) in items" :key="index">{{item.title}}</th>
          </tr>
        </thead>
        <tbody class="table__tbody tbody">
          <tr class="tbody__row">
            <td class="tbody__col" v-for="(item,index) in items" :key="index">{{item.body}}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>
</template>

<script>
export default {
  name: "Project",
  data() {
    return {
      title: "اطلاعات تحصیلی",
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
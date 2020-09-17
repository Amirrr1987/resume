<template>
  <section class="education">
    <div class="education__container">
     <h3 class="education__title">{{title}} :</h3>
      <table class="education__table table">
        <thead class="table__thead thead">
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
  name: "Education",
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
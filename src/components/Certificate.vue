<template>
  <section class="certificate">
    <div class="certificate__container">
     <h3 class="certificate__title">{{title}} :</h3>
      <table class="certificate__table table">
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
  name: 'Certificate',
  data() {
    return {
      title: "مدارک",
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
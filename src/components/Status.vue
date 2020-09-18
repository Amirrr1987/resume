<template>
  <section class="status">
    <div class="status__container">
     <h3 class="status__title">{{title}} :</h3>
      <table class="status__table table">
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
  name: "Status",
  data() {
    return {
        title: 'اطلاعات شغلی',
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
      ],
    };
  },
};
</script>
<template>
  <section class="basic">
    <div class="basic__container">
      <h3 class="basic__title"><i class="icon icon--info-1"></i> {{title}} :</h3>
      <table class="basic__table table">
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
  name: 'Basic',
  data() {
    return {
      title: 'اطلاعات پایه',
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
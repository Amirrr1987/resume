<template>
  <table class="table">
    <tr class="table__row">
      <th class="table__col">{{title}} :</th>
    </tr>
    <tr class="table__row">
      <th class="table__col" v-for="(item,index) in items" :key="index">{{item.title}}</th>
    </tr>
    <tr class="table__row">
      <td class="table__col" v-for="(item,index) in items" :key="index">{{item.body}}</td>
    </tr>
  </table>
</template>

<script>
export default {
  name: 'BackEndLang',
  data() {
    return {
      title: 'BackEndLang',
      items: [
        {
          title: "نام",
          body: "امیر",
        },
        {
          title: "تاریخ تولد",
          body: "1366",
        },
        {
          title: "وضیعت تاهل",
          body: "متاهل",
        },

        {
          title: "وضعیت سربازی",
          body: "اتمام خدمت",
        },
      ],
    };
  },
};
</script>
<template>
  <section class="links">
    <div class="links__container">
      <table class="links__table table">
        <thead class="table__thead thead">
          <tr class="thead__row">
            <th class="thead__col thead--title" colspan="4">{{title}} :</th>
          </tr>
        </thead>
        <tbody class="table__tbody tbody">
          <tr class="tbody__row">
            <td class="tbody__col" v-for="(item,index) in items" :key="index">
                {{item.img}}
                {{item.url}}
                {{item.title}}
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>
</template>

<script>
export default {
  name: "Links",
  data() {
    return {
      title: "پیوندها",
      items: [
        { 
          title: "نام" ,
          img  : "امیر",
          url  : "امیر",
        },

      ],
    };
  },
};
</script>
<template>
  <section class="links">
    <div class="links__container">
     <h3 class="links__title">{{title}} :</h3>
      <table class="links__table table">
          <tr class="table__row">
            <td class="table__col" v-for="(item,index) in items" :key="index">
                {{item.img}}
                {{item.url}}
                {{item.title}}
            </td>
          </tr>
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
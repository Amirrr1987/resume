<template>
  <section class="description">
    <div class="description__container">
     <h3 class="description__title"><i class="icon icon--commenting-o"></i>{{title}} :</h3>
      <table class="description__table table">
          <tr class="table__row">
            <td class="table__col">{{description}}</td>
          </tr>
      </table>
    </div>
  </section>
</template>

<script>
export default {
  name: "Description",
  data() {
    return {
      title: "توضیحات",
      description: "ghfhghgffghh",
    };
  },
};
</script>
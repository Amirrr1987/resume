<template>
  <section class="description">
    <div class="description__container">
     <h3 class="description__title">{{title}} :</h3>
      <table class="description__table table">
        <tbody class="table__tbody tbody">
          <tr class="tbody__row">
            <td class="tbody__col">{{description}}</td>
          </tr>
        </tbody>
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
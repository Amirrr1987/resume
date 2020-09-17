<template>
  <section class="description">
    <div class="description__container">
      <table class="description__table table">
        <thead class="table__thead thead">
          <tr class="thead__row">
            <th class="thead__col thead--title" colspan="4">{{title}} :</th>
          </tr>
        </thead>
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
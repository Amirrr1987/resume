<template>
  <section class="basic">
    <div class="basic__container">
      <table class="basic__table table">
        <thead class="table__thead thead">
          <tr class="thead__row">
            <th class="thead__col thead--title" colspan="4">اطلاعات پایه :</th>
          </tr>
          <tr class="thead__row">
            <!-- <th class="thead__col" v-for="(item,index) in items" :key="index">{{item.title}}</th> -->
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
  name: "Basic",
  data() {
    return {
      items: null,
    }
  },
  mounted () {
    axios
      // .get('https://api.coindesk.com/v1/bpi/currentprice.json')
      .get('@/assets/json/basic.json')
      
      .then(response => (this.items = response.data))
      // console.log(this.info);
    
  }
  


};
</script>

<style>
</style>
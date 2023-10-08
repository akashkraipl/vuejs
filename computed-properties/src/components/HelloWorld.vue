<script>
export default {
  data(){
    return {
      dollar: 100,
      currentRsPrice: 80
    }
  },
  computed: {
    convertToRupees: function(){
      return this.dollar*this.currentRsPrice;
    }
  }
}
</script>

<template>
  <h1>Computed properties</h1>
  <p>we can use template expression or methods but it is not correct way because these calculate value every time</p>
  <p>computed value also cache</p>
  <h2>Dollar value :- {{ dollar }}</h2>
  <h2>In Rupees :- {{ convertToRupees }}</h2>
</template>

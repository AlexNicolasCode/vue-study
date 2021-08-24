<template>
  <h2>Filters Study</h2>

  <div>
    <p>{{ currencyUSD(coin) }}</p>
  </div>
</template>

<script>
export default {
  name: 'Filter',
  data() {
    return {
      coin: null,
    }
  },
  methods: {
    currencyUSD(value) {
      return '$ ' + value
    }
  },
  mounted () {
    fetch('https://api.coindesk.com/v1/bpi/currentprice.json')
      .then(async (res) => {
        const data = await res.json();
        this.coin = data.bpi.USD.code;
      })
  }
}

</script>
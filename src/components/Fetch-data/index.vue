<template>
  <h2>Fetch data Study</h2>

  <div>
    <p>Dollar: {{ coin }}</p>
  </div>
</template>

<script>
export default {
  name: 'FetchData',
  data() {
    return {
      coin: null,
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
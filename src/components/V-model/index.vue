<template>
  <h2>V-Model Study</h2>

  <div>
    <input v-model="message" />
    <p>{{ message }}</p>
  </div>

  <div>
    <select v-model="props">
      <option>1</option>
      <option>2</option>
      <option>3</option>
    </select>

    <p>{{ props }}</p>
  </div>
</template>

<script>
export default {
  name: 'Vmodel',
  data() {
    return {
      message: '',
      props: '1',
      counter: 0,
    }
  },
  methods: {
    say: (msg) => {
      alert(msg)
    }
  }
}

</script>
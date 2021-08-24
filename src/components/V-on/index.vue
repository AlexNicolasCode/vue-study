<template>
  <h2>V-On Study</h2>

  <div>
    <button v-on:click="counter += 1">+</button>
    <button v-on:click="counter--">-</button>
    <div>{{ counter }}</div>

    <button 
      v-on:click="say('action')" 
      v-on:keyup.enter="say('action')"
    >
      Action
    </button>

    <button>Als</button>
  </div>
</template>

<script>
export default {
  name: 'Von',
  data() {
    return {
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
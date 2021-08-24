<template>
  <h2>V-Bind Study</h2>

  <div>
    <img v-bind:src="image" alt="image">
  </div>
</template>

<script>
export default {
  name: 'Vbind',
  data() {
    return {
      image: 'https://w7.pngwing.com/pngs/738/264/png-transparent-angularjs-react-vue-js-javascript-library-others-thumbnail.png'
    }
  },
}

</script>
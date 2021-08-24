<template>
  <h2>V-for and V-if Study</h2>

  <div>
    <ul v-if="list.length > 3">
      <li v-for="(value, index) in list" :key="value">
        {{ index }}
        {{ value.title }}
        {{ value.author }}
        {{ value.publishedAt }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'List',
  data() {
    return {
      counter: 0,
      list: [
        {
          title: 'Como fazer listas no Vue',
          author: 'Jane Doe',
          publishedAt: '2016-04-10'
        },
        {
          title: 'Como fazer listas no Vue',
          author: 'Jane Doe',
          publishedAt: '2016-04-10'
        },
        {
          title: 'Como fazer listas no Vue',
          author: 'Jane Doe',
          publishedAt: '2016-04-10'
        },
        {
          title: 'Como fazer listas no Vue',
          author: 'Jane Doe',
          publishedAt: '2016-04-10'
        },
      ]
    }
  },
  methods: {
    say: (msg) => {
      alert(msg)
    }
  }
}
</script>
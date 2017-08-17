<template>
  <div class="login">
    <h1 v-text='title'></h1>
    <ul>
      <li v-for='item in items' :class='{finished: item.isFinishes}'>{{item.label}}</li>
    </ul>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        // kk
        title: 'this is a todo list',
        items: [
          {
            label: 'coding',
            isFinished: false,
            isFinishes: false
          },
          {
            label: 'coding',
            isFinished: true,
            isFinishes: true
          }
        ],
        liClass: 'thisisliClass'
      }
    },
    methods: {
      // kk
    }
  }
</script>
<style>
.finished {
  text-decoration: underline;
}

</style>



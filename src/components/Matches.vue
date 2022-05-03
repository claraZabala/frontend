<template>
  <div id="app">
    <h1> {{ message }} </h1>
    <button class="btn btn-success btn-lg" @click="buyTicket"> Buy ticket </button>
    <h4> Total tickets bought: {{ tickets_bought }} </h4>
  </div>
</template>

<script>

export default {
  name: 'CaCa',
  data () {
    return {
      message: 'My first component',
      tickets_bought: 0
    }
  },
  methods: {
    buyTicket () {
      this.tickets_bought += 1
    }
  }
}

</script>
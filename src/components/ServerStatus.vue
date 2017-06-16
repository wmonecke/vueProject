<template>
  <div>
    <p>Server Status: {{ status }}</p>
    <hr>

    <div>
      <button v-on:click="changeStatus" type="button" name="button">Change</button>
    </div>
    <hr>
  </div>
</template>

<script type="text/javascript">
  export default {
    data: function () {
      return {
        status: 'Critical'
      }
    },
    methods: {
      changeStatus: function () {
        this.status = 'Normal'
      }
    }
  }
</script>

<style media="screen">

</style>

<template>
  <div>
    <h2 class="text-center">Video Search</h2>
    <br />
    <input @input="onInput" placeholder="Search for..." class="form-control" />
  </div>
</template>

<script>
export default {
  name: 'SearchBar',
  methods: {
    onInput: function(event) {
      this.$emit('termChange', event.target.value);
    },
  },
};
</script>

<style scoped>
input {
  width: 40%;
  margin: 0 auto;
}
div {
  text-align: center;
  margin: 20px;
}
</style>

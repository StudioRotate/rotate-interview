<template lang="html">
  <div class="">
    <select class="Dropdown__button" name="">
      <option v-for="val in values" v-bind:value="val">{{ val }}</option>
    </select>
    </div>
</template>

<script>
export default {
  name: 'Dropdown',
  props: ["values"],
  data() {
    return {
    }
  }
}
</script>

<style lang="css">
.Dropdown__button {
  width: 330px;
  border-radius: 50px;
  padding: 17px 0;
  font-size: 11px;
  background-color: #FFFFFF;
  text-align-last: center;
}
</style>

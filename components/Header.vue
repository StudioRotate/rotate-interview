<template>
<section class="Header">
  <div class="Header_Wrapper">
  <img src="imgs/logo-large.svg" alt="Logo" class="Logo">
  </div>
</section>
</template>

<script>
export default {
name: 'Header'
}
</script>
<style>
  .Header {
    position: fixed;
    width: 100%;
    padding-top: 25px;
    padding-right: 30px;
    padding-bottom: 50px;
    padding-left: 30px;
  }

  .Header_Wrapper {
    display: flex;
    flex: column nowrap;
    align-items: center;
    height: 16px;
    width: 137px;
    margin: 0 auto;
    padding-top: 25px;
    padding-right: 30px;
    padding-bottom: 50px;
    padding-left: 30px;
  }

</style>

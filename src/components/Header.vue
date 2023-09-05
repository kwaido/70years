<script setup>
  import Modal from './Modal.vue';
  import { ref, watch} from 'vue'


  const isModalVisible = ref(false);
  
  function toggleModal () {
    isModalVisible.value = !isModalVisible.value

  }
  
  watch(isModalVisible, () => {
    document.body.classList.toggle('overflow-hidden');
  })

</script>

<template>

<header class="header">

<Modal 
  v-if="isModalVisible"
  @response="toggleModal"
/>

<div class="container">
  <div class="header-line">
    <div class="header-logo">
      <img src="/src/assets/logo-header.svg" alt="logo">
      <img src="/src/assets/text-header.svg" alt="name">
    </div>
    <button @click="toggleModal" class="header-menu">меню</button>
  </div>
</div>

</header>

</template>

<style scoped>

.header {
  position: absolute;
  left: 0;
  right: 0;
}

.header-line {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 40px;
}

.header-logo img:nth-child(1) {
  margin-right: 16px;
}

.header-menu {
  color: #000;
  text-align: center;
  font-family: Unbounded;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  letter-spacing: -0.54px;

  width: 100px;
  height: 50px;
  background-color: #fff;
  border: 0;
  border-radius: 99px;
  padding: 8px 16px;
  cursor: pointer;
}

.overflow-hidden {
  height: 100% !important;
  width: 100% !important;
  position: relative !important;
  overflow: hidden !important;
}

/* TEST */



/* TEST */

</style>
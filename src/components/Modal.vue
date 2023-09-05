<script setup> 
import { ref, onMounted, onBeforeUnmount } from 'vue';

const emit = defineEmits(['response'])

function closeModal () {
  emit('response')
}

const modal = ref()

onMounted( () => {
  setTimeout(() => {
    modal.value.classList.add('active')
  })
})

</script>

<template> 
  <div @click="closeModal" class="modal-bg"></div>
  <div ref="modal" class="modal">
    <div class="modal-inner">
      <button @click="closeModal" class="close">закрыть</button>
      <div class="menu-items">  
        <span class="item"><a href="#">Афиша</a></span>
        <span class="item"><a href="#">Проекты 70</a></span>
        <span class="item"><a href="#">Конкурс/флешмобы</a></span>
        <span class="item"><a href="#">Брендбук 70 летия</a></span>
      </div>
    </div>
  </div>
</template>

<style>


a {
  text-decoration: none;
  color: #FFF;
  text-align: center;
  font-family: Unbounded;
  font-size: 32px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  letter-spacing: -0.96px;
}

.modal-bg {
  height: 100vh;
  width: 100vw;
  position: absolute;
  z-index: 2;
}

.modal {
  background-color: #A1E224;
  height: 100vh;
  width: 45%;
  position: absolute;
  right: -100%;
  z-index: 3;
  border-radius: 40px 0 0 40px;
  
  transition: right 1s 1s ;


}

.modal-inner {
  height: 100%;
  display: flex;
  flex-direction: column;
}

.close {
  color: #000;
  text-align: center;
  font-family: Unbounded;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  letter-spacing: -0.54px;

  width: 120px;
  height: 48px;
  margin-top: 40px;
  margin-right: 48px;
  border: 0;
  border-radius: 99px;
  align-self: flex-end;
  cursor: pointer;
}

.menu-items {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  padding: 0 10px 82px 77px; 
}

.item {
  margin-bottom: 32px;
}

.active {
  right: 0; 
  transition: right 1s;
}


</style>
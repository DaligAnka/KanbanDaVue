<script setup>
// import HelloWorld from './components/HelloWorld.vue'
import { VueDraggableNext } from 'vue-draggable-next';
</script>

<template>

  <div class="kanban">
<div class="column-container column-container1">
<div class="column-header">
<span class="column-title"> Необработанные </span>
<button class="column-filterBtn"> Filter me </button>
</div>

<VueDraggableNext  class="task-column">
            </VueDraggableNext>

</div>

<div class="column-container column-container2">
  <div class="column-header">
    <span class="column-title"> В работе </span>
    <button class="column-filterBtn"> filter me </button>
  </div>

  <VueDraggableNext  class="task-column">
            </VueDraggableNext>

</div>


<div class="column-container column-container3">
  <div class="column-header">
    <span class="column-title"> Завершённые</span>
    <button class="column-filterBtn"> filter me </button>
  </div>

  <VueDraggableNext  class="task-column">
            </VueDraggableNext>

</div>

            </div>

</template>

<style scoped>
.kanban {
    display: flex;
    flex-direction: row;
}
.column-container {
    display: flex;
    flex-direction: column;
    /* width: fit-content; */
    width: 100%;
    border-radius: 25px;
    height: fit-content;
    margin-right: 10px;
    margin-left: 10px;
    padding: 0 15px;
}
.column-container1 {
    background-color: blue;
}
.column-container2 {
    background-color:  #abe574;;
}
.column-container3 {
    background-color: pink;
}
.column-header {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin: 20px 0;
}
.column-title {
    text-align: center;
    font-size: 24px;
    font-weight: 600;
}
.task-column {
    list-style: none;
    margin: 0;
    padding: 0;
    /* min-height: auto; */
    min-height: 100vh;
}
.column-filterBtn {
margin-left: auto;

}

</style>

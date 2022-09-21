<template>
  <teleport to=".modals-container"> 
  <div
  class="modal"
  >
    <h1>This is a modal</h1>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eius doloribus dolores aliquid non quisquam, illum, temporibus ipsa deleniti consectetur laboriosam explicabo perspiciatis modi quod necessitatibus ipsum nemo? Assumenda, commodi necessitatibus.</p>
    <button>Hide modal</button>
  </div>
  </teleport>
</template>


<style>
  .modal {
    background: purple;
    padding: 10px;
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    z-index: 1;
  }
</style>
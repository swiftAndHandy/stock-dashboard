<template>
    <div class="card">
      <!-- Füge hier den Inhalt der Karte ein -->
      <slot></slot>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Cards',
  }
  </script>
  
  <style scoped>
  .card {
    background: #011F35;
    padding: 20px 32px;
    gap: 20px;
    border-radius: 16px 0px 0px 0px;
  }
  </style>
 <template>
    <div>
      <button @click="increment">Cliquez-moi</button>
      <p>Nombre de clics : {{ count }}</p>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'

  const count = ref(10)
  function increment() {
    count.value++
  }
  </script>
  
  <style scoped>
  button {
    font-size: 1.2em;
    padding: 10px;
    margin: 10px;
    background-color: aqua;
    border-radius: 10px;
    width: 50%;
  }
  
  p {
    font-size: 1.2em;
  }
  
  </style>

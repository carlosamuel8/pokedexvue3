
<!-- vmodel -->
<!-- <script setup>
import { ref } from 'vue'

const nome = ref('fulano')


</script>

<template>
  <div class="col-6">
    <span>{{ nome }}</span>
    <br>
    <input type="text" v-model="nome">
  </div>
</template>

<style scoped>

</style> -->

<!-- vif -->
<!-- <script setup>
import { ref } from 'vue'

const show = ref(true)




</script>

<template>
  <div class="col-6">
    <span v-if="show">Olá pessoas</span>
    <span v-else>Sem ninguém</span>
    <button @click="show = !show">Mostrar/Ocultar</button>

  </div>
</template>

<style scoped>

</style> -->

<!-- <script setup>
import { computed, ref } from 'vue'

const media = ref(0)
const nota1 = ref(0)
const nota2 = ref(0)

const calcularMedia = computed(() => {
  media.value = (nota1.value + nota2.value) / 2
})


</script>

<template>
  <div class="flex">
    <span>Nota 1</span>
    <input type="number" v-model="nota1">
    <br>
    <br>
    <span>Nota 2</span>
    <input type="number" v-model="nota2">
    <br>
    <button @click="calcularMedia">calcular </button>
    <span>{{ media }}</span>
  </div>
</template>

<style scoped>

</style> -->


<script setup>
import { computed, ref } from 'vue'

const array = ref([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
</script>

<template>
  <div class="flex">
    <ul>
      <li v-for="item in array" 
      :key="item">
      {{ item }}
      </li>
      
    </ul>
  </div>
</template>

<style scoped>

</style>
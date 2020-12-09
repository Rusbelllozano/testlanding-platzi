<template>
  <div class="grid grid-cols-2 bg-blue-900 p-20 text-white">
    <div class="">
      <div>
        <h1 class="text-6xl leading-tight font-black">
          Formate online como profesional en tecnologia
        </h1>
      </div>
      <div class=" my-6 text-lg">
        <h4 class="">
          <strong>70% </strong> de los graduados de Platzi
          <strong>duplican</strong> sus <strong>ingresos</strong>
        </h4>
        <h4 class="">
          <strong>20%</strong> crean su propia empresa de tecnología o startup
        </h4>
      </div>

      <p class="mb-3">Acelera tu carrera profesional:</p>
      <div class="flex flex-row px-4">
        <input
          type="text"
          class="p-3 rounded mr-2 border border-white bg-gray-800 flex flex-auto"
          placeholder="Escribe tu correo electronico"
        />
        <button class="bg-green-500 rounded text-gray-900 p-3 font-extrabold">
          ENTRA A PLATZI
        </button>
      </div>
      <p class="mt-8 text-gray-200">
        Al ingresar aceptas
        <a class="text-blue-400" href="">Términos de Servicio</a>
        y
        <a class="text-blue-400" href="">Políticas de privacidad</a>
      </p>
    </div>
    <div class="grid grid-rows-2 grid-flow-col gap-4 items-center">
        <img v-for="(person,index) in personas" :key="index" class="w-25 h-25 rounded" :src="person" alt="">
    </div>
  </div>
</template>
<script>
export default {
    data(){
        return {
            personas:[
            "https://static.platzi.com/media/teachers/diego-de-granda.jpg",
            "https://static.platzi.com/media/teachers/rosa-morel.jpg",
            "https://static.platzi.com/media/teachers/sebastian-sosa.jpg",
            "https://static.platzi.com/media/teachers/teachers/276-daniela-belen-gonzalez",
            "https://static.platzi.com/media/teachers/liliana-zamacona.jpg",
            "https://static.platzi.com/media/teachers/Screen_Shot_2020-06-10_at_6.56.58_PM.png",
            "https://static.platzi.com/media/teachers/teachers/132-nicole-chapaval"

        ]
        }
        
    }
};
</script>
<style></style>

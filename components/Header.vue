<template>
    <nav class="w-full h-12 bg-blue-500 flex flex-row">
        <div class="flex flex-none items-center p-3 mr-1">
            <img class="h-6 m-1" src="https://static.platzi.com/mf-landings/image/isotipoPlatzi-442ccc1186a9806e18c9889cc301ffe1.png" alt="">
            <img class="h-6" src="https://static.platzi.com/mf-landings/image/logotipo-platzi-768799552e5f26369e21a807b8a533f7.png" alt="">
        </div>
        <div class="flex ml-auto">
            <!-- <div class="flex items-center">
                <div class="flex flex-none text-white bg-red-500 p-1 font-bold rounded-l-lg animate-pulse text-sm">LIVE</div>
                <div class="flex w-9 max-w-md truncate text-white p-1  bg-gray-500 rounded-r-lg text-sm">
                  <p>¿Cómo distribuir tu tiempo para alcanzar a hacer todo?</p> 
                </div>
            </div> -->
            <div class="flex p-2 items-center ">
                <ul class="flex flex-row text-white space-x-4 border-r-2 border-white mr-2">
                    <li v-for="(nav,index) in mainMenu" :key="index">
                        <p class="font-bold hover:opacity-50 cursor-pointer">
                            {{nav}}
                        </p>
                    </li>
                    <li></li>
                </ul>
                <div class="text-md text-white flex flew-row mx-3 cursor-pointer">
                    <p>Iniciar mi plan</p>
                    <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg>
                </div>
                <div class="">
                    <button class="bg-green-600 rounded-lg p-1 cursor-pointer transition duration-500 hover:shadow-md">
                        <p class="text-sm">Iniciar sesión</p>
                    </button>
                </div>
                <div>
                    <form action="" class="flex ml-5 h-8">
                        <input class="flex rounded-l-md bg-blue-900 px-3" type="text" placeholder="Buscar en platzi">
                        <button class="flex w-10 bg-green-600 rounded-r-md p-1 text-sm justify-center items-center cursor-pointer">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path></svg>
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </nav>
</template>
<script>
export default {
    
    data(){
        return{
            mainMenu:[
                "Cursos",
                "Blog",
                "Foro",
                "Agenda",
                "TV",
                "Contactanos"
            ]
        }
    }
}
</script>
<style>
    .img-logo{
        height: 25px;
    }
</style>
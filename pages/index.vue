<template>
  <div class="flex h-screen bg-black p-1">
    <div class="w-3/12 h-full flex flex-col">
      <div class="h-64 bg-blue-500 border-2 border-black rounded">
        <div class="flex rounded-lg p-4">
          <img class="h-16 w-16 rounded-full mx-2 shadow" src="~/assets/img/uc.jpg" alt="img">
          <div class="text-left">
            <div class="text-gray-200 uppercase text-xs">Cuerpo de bomberos</div>
            <h2 class="text-lg text-white tracking-widest uppercase font-semibold">Temuco</h2>
            <div class="text-gray-200 text-xs">Cuartel 4ta compañia</div>
          </div>
        </div>
      </div>
      <div class="h-full bg-gray-100 border-2 border-black rounded">
        <div class="p-4">
          <h4 class="text-gray-700 text-center">Autenticación con DNI y contraseña</h4>
          <label class="block mb-4">
            <span class="sr-only">DNI</span>
            <input class="form-input mt-1 block w-full" placeholder="DNI">
          </label>
          <label class="block mb-4">
            <span class="sr-only">Contraseña</span>
            <input class="form-input mt-1 block w-full" type="password" placeholder="Contraseña">
          </label>
          <button class="bg-orange-500 hover:bg-orange-700 w-full text-white font-bold py-2 px-4 rounded">
            Ingresar
          </button>
        </div>
      </div>
      <div class="h-full bg-gray-100 border-2 border-black rounded">
        QR Code
      </div>
    </div>
    <div class="w-5/12 h-full">
      <div class="h-full p-4 flex flex-col items-center justify-start bg-gray-100 border-2 border-black rounded">
        <span
          class="p-2 mb-4 rounded-full text-orange-600 text-xs uppercase font-semibold">Personal presente</span>
        <div v-for="aux in team" class="bg-white rounded my-1 px-4 w-full">


          <div class="flex rounded-lg p-4">
            <img class="h-8 w-8 rounded-full mx-2 shadow" :src="`/img/${aux.icon}`" alt="img">
            <div class="flex justify-between items-center w-full">
              <div class="text-left">
                <div class="text-gray-700 uppercase text-xs font-bold">{{ aux.name }}</div>
                <div class="text-green-700 text-xs">Guardia nocturna</div>
              </div>
              <div>
                <div class="text-gray-500 text-xs">presente hace 21 horas</div>
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>
    <div class="w-4/12 h-full flex flex-col">
      <div class="h-full bg-gray-100 border-2 border-black rounded">
        Mapa
      </div>
      <div class="h-full bg-gray-100 border-2 border-black rounded">
        Emergencias
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      team: [
        {name: 'Samir Valls', icon: 'firefighter-80.png'},
        {name: 'Virginia Jover', icon: 'fireman-female-80.png'},
        {name: 'Damian Morales', icon: 'firefighter-80.png'},
        {name: 'Luciano Hervas', icon: 'firefighter-80.png'},
        {name: 'Faustino Mata', icon: 'firefighter-80.png'},
        {name: 'Paula Contreras', icon: 'fireman-female-80.png'},
      ]
    }
  }
};
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
  "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

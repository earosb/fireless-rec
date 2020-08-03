<template>
  <div class="flex">
    <div class="flex flex-col w-full h-screen bg-blue-100">
      <div class="h-64 bg-blue-500">
        <img
          class="h-24 rounded-full p-2"
          src="~/assets/img/uc.jpg"
          alt="Logo 4ta cia"
        />
        <div class="flex flex-col justify-center pl-4">
          <h1 class="text-xl font-bold">Cuartel 4ta Compañia</h1>
          <h2 class="text-base uppercase">Cuerpo de bomberos de Temuco</h2>
        </div>
      </div>
      <div class="h-full bg-blue-100">2</div>
      <div class="h-full bg-blue-500">3</div>
    </div>
    <div class="w-full h-screen bg-green-100"></div>
    <div class="w-full h-screen bg-red-100"></div>
  </div>
</template>

<script>
export default {};
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

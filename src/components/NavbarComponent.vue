<template>
  <nav
    class="w-64 min-h-screen h-full p-5 bg-stone-900 shadow-xl border-r border-stone-800 items-center text-white text-center">

    <div class="mb-4 border-fuchsia-800">
      <img
        src="https://media.licdn.com/dms/image/v2/D4D03AQHHG7IKSvVm2g/profile-displayphoto-shrink_800_800/B4DZQ9f3D9GUAc-/0/1736198550795?e=1753315200&v=beta&t=n3ldUKQwsW3fretO-wrv6BX9Nd_lN22UQD6gPPU4ZUM"
        alt="Foto de perfil" class="w-48 h-48 rounded-full border-4 border-fuchsia-800 shadow-lg" />
      <h1 class="mt-3 text-lg font-bold text-shadow-lg">Vinícius Gualtieri Moraes</h1>
    </div>

    <div class="w-full">
      <ul>
        <router-link to="/"
          class="block mb-2 p-2 border border-fuchsia-700 shadow-lg text-white text-center hover:border-fuchsia-900 hover:bg-fuchsia-800">
          Início
        </router-link>
        <router-link to="/sobre"
          class="block mb-2 p-2 border border-fuchsia-700 shadow-lg text-white text-center hover:border-fuchsia-900 hover:bg-fuchsia-800">
          Sobre
        </router-link>
        <router-link to="/contato"
          class="block mb-2 p-2 border border-fuchsia-700 shadow-lg text-white text-center hover:border-fuchsia-900 hover:bg-fuchsia-800">
          Contato
        </router-link>
      </ul>
    </div>
  </nav>
</template>
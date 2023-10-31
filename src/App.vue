<template>
  <div class="flex flex-col min-h-screen">
    <header class="flex items-center border-b border-gray-600">
      <router-link to="/profile" class="p-4 mr-3 text-green-500 text-2xl">
        <i class="fas fa-user"></i>
      </router-link>
      <h1 class="text-white font-black text-xl">{{ $route.name }}</h1>
    </header>
    <main>
      <router-view />
    </main>
    <footer></footer>
  </div>
</template>
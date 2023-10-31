<template>
  <div class="flex flex-col min-h-screen">
    <header>
      <router-link to="/profile">
        <i class="fas fa-user"></i>
      </router-link>
    </header>
    <main>
      <router-view />
    </main>
    <footer></footer>
  </div>
</template>
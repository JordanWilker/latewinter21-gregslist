<template>
  <div class="app">
    <header class="container-fluid bg-danger text-light">
      <div class="row">
        <div class="col text-center">
          <h1>Gregslist</h1>
          <div class="text-light">
            <router-link :to="{name: 'Home'}">Home</router-link> |
            <router-link :to="{name: 'Cars'}">Cars</router-link> |
            <router-link :to="{name: 'HousesPage'}">Houses</router-link> |
            <router-link :to="{name: 'JobsPage'}">Jobs</router-link>

          </div>
        </div>
      </div>
    </header>
    <main>
      <router-view />
    </main>
    <footer class="container-fluid bg-info text-light">
      <div class="row">
        <div class="col text-center">
          <p class="m-3">
            Made with <img alt="Vue logo" src="./assets/logo.png" /> by
            codeworks
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>
<style>
.app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

main {
  flex-grow: 1;
}

footer img {
  width: 1em;
}

a {
  color: white;
}
</style>

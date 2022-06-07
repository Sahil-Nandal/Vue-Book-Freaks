<template>
  <header>
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-0evHe/X+R7YkIZDRvuzKMRqM+OrBnVFBL6DOitfPri4tjfHxaWutUpFmBp4vmVor"
      crossorigin="anonymous"
    />
  </header>
  <!-- NAVIGATION BAR -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <a style="margin-left: 50px" class="navbar-brand" href="#">BOOK FREAKS! </a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNavDropdown"
      aria-controls="navbarNavDropdown"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
      <ul class="navbar-nav">
        <li class="nav-item active">
          <a class="nav-link" href="#/">Home </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#/novels">Novels</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#/biographies">Biographies</a>
        </li>
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            href="#"
            id="navbarDropdownMenuLink"
            role="button"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >
            Your Inputs
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
            <a class="dropdown-item" href="#">Find your match</a>
            <a class="dropdown-item" href="#">Review a Book</a>
            <a class="dropdown-item" href="#">What are you reading?</a>
          </div>
        </li>
        <li class="nav-item dropdown">
          <a
            class="nav-link dropdown-toggle"
            href="#"
            id="navbarDropdownMenuLink"
            role="button"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >
            Select your Niche!
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
            <a class="dropdown-item" href="#">Physics</a>
            <a class="dropdown-item" href="#">Self Help</a>
            <a class="dropdown-item" href="#">Biography</a>
            <a class="dropdown-item" href="#">Science Fiction</a>
            <a class="dropdown-item" href="#">Business and Entrepreneurship</a>
          </div>
        </li>
      </ul>
    </div>
  </nav>
  <div id="app">
    <Home data="Sam:" msg="Welcome to the first app!" />
  </div>
  <component :is="currentView" />
</template>

<script>
import home from './components/home.vue';
import novels from './components/novels.vue';
import biographies from './components/biographies.vue';

const routes = {
  '/': home,
  '/novels': novels,
  '/biographies': biographies,
};

export default {
  data() {
    return {
      currentPath: window.location.hash,
    };
  },
  computed: {
    currentView() {
      return routes[this.currentPath.slice(1) || '/'] || NotFound;
    },
  },
  mounted() {
    window.addEventListener('hashchange', () => {
      this.currentPath = window.location.hash;
    });
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

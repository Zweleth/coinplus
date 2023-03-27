<template lang="">
  <header>
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <a class="navbar-brand" href="#"
          ><i class="fa-brands fa-bitcoin"></i>Coinplus</a
        >
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
                <router-link to="/home">Home</router-link>
            </li>
            <li class="nav-item">
                <router-link to="/signin">Sign in</router-link>
            </li>
            <li class="nav-item">
                <router-link to="/signup">Sign up</router-link>
            </li>
            <li class="nav-item">
                <router-link to="/about">About us</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>
<script>
export default {
    name: 'navbar'
};
</script>
<style scoped>
header {
    position: fixed;
    width: 100vw;
    z-index: +5;
}

.navbar {
    color: gray;
    background-color: #222;
}

.navbar a {
    color: gray;
    text-decoration: none;
}
.navbar-nav a.router-link-exact-active {
    color: aqua;
  }

.navbar a:hover {
    animation: linkHover 0.4s ease-in-out forwards;
}

.navbar-nav {
    margin-left: auto;
    margin-right: 2rem;
    gap: 1.5rem;
}

.navbar-brand {
    padding-left: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
}

.fa-bitcoin {
    margin-right: 0.4rem;
    display: block;
    scale: 1.2;
}

</style>

<script setup>
const className = 'WD19312'
const time = '30h'
const status = 0;//1 là đang hoạt động, 0 là ngừng hoạy động

// const time = '30h'
// const time = '30h'
// import HelloWorld from './components/HelloWorld.vue'
// import HelloWorld from './views/bai2'
// import bai2 from './views/bai2.vue'
// import { RouterView } from 'vue-router';
</script>

<template>
 <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <RouterLink to="/product">product</RouterLink>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Features</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
  
<!-- </ul> -->
  <!-- </ul>
  <h1 class="">{{ className }}</h1>
  <table class="table">
  <thead>
    <tr>
      <th scope="col">Stt</th>
      <th scope="col">Tên</th>
      <th scope="col">Thời gian</th>
      <th scope="col">Trạng thái</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>{{ className }}</td>
      <td>{{ time }}</td>
      <td>{{ status == 1 ? "Đang hoạt động" : "Ngừng hoạt động" }}</td>
    </tr>
    
  </tbody>
</table> -->
  <!-- <button class="btn btn-primary">Đăng nhập</button>
<bai2/> -->
<router-view/>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>

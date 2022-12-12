<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <div class="container">
        <a class="navbar-brand">Vue Blog</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
            <li class="nav-item">
            <a><router-link :to="{name: 'Home'}" class="nav-link">Anasayfa</router-link></a>
            </li>
            <li class="nav-item">
            <a><router-link :to="{name: 'About'}" class="nav-link">Hakkında</router-link></a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script></script>
<style>
nav{
    background-color: #2c3e50;
    box-shadow: 0 12px 20px 0 #055f41, 0 6px 12px 0 #2387f9;
}
a{
    text-decoration: none;
}
a.router-link-active{
    color: #42b983 !important;
}
</style>

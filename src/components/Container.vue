<template>
  <div class="bg-dark py-5">
    <div class="container px-5">
      <div class="row gx-5 justify-content-center">
        <div class="col-lg-6">
          <div class="text-center my-5">
            <img alt="Vue logo" src="../assets/logo.png" />
            <h1 class="display-5 fw-bolder text-white mb-2">
              Vue.js ile ilgili blog yazıları
            </h1>
            <p class="lead text-white-50 mb-4">
              Öğrenme sürecinde doküman okumanın yanında blog yazıları okuyarak
              gelişiminizi hızlandırabilirsiniz!
            </p>
            <div class="d-grid gap-3 d-sm-flex justify-content-sm-center">
              <router-link :to="{ name: 'Post' }">
                <a class="buton btn btn-outline-dark btn-lg px-4 me-sm-3">
                  Yayınlanmış yazılar
                </a>
              </router-link>
              <router-link :to="{ name: 'AddPost' }"><a class="buton btn btn-outline-dark btn-lg px-4">
                Yeni bir yazı yayınla!
              </a></router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style>
 .buton{
  box-shadow: 0 12px 20px 0 #055f41, 0 6px 12px 0 #2387f9;
  color: #999;
 }
 .buton:hover{
  color: #fff;
 }
</style>

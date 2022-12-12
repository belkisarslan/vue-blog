<template>
  <div>
    <div class="card bg-dark mb-4">
      <div class="card-body p-4">
        <div class="d-flex justify-content-center">
          <div class="ms-4">
            <h3>{{post.title}}</h3>
            <p class="mb-1">
              {{post.message}}
            </p>
            <div class="small text-muted">- {{post.name}}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
 export default {
    props: ["post"],
    setup(props){
      
    }
 }
</script>

<style>
 .card{
   color:#fff;
   border: none;
   background-color: #2c3e50;
    box-shadow: 0 12px 20px 0 #055f41, 0 6px 12px 0 #2387f9;
}
</style>
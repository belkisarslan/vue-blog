<template>
    <div class="py-5 border-bottom">
        <div class="container px-5 my-5 px-5">
                <div class="text-center mb-5">
                    <h2 class="fw-bolder">Sizden Gelenler</h2>
                    <p class="lead mb-0">Vue hakkında yorumlar, yenilikler, gelişmeler</p>
                </div>
                <div class="row gx-5 justify-content-center">
                    <div class="col-lg-6">
                        <!-- deneme yazı-->
                        <div v-for="post in posts" class="card mb-4">
                            <div class="card-body p-4">
                                <div class="d-flex">
                                    <div  class="ms-4">
                                        <h3>vue</h3>
                                        <p class="mb-1">Thank you for putting together such a great product. We loved working with you and the whole team, and we will be recommending you to others!</p>
                                        <div class="small text-muted">- Nick Name, Location</div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
    </div>
</template>
<script>
import { ref } from "vue"
import GetPost from "../composables/GetPost";
export default {
    setup() {
    const posts = ref();
    GetPost().then((data) => {
      posts.value = data;
    });
    console.log(posts)
    return  {posts} ;
    }
}
</script>
<style>
    
</style>
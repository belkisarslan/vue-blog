<template>
    <div class="post bg-dark py-5 border-bottom">
        <div class="container px-5 my-5 px-5">
                <div class="text-center mb-5">
                    <h2 class="fw-bolder">Sizden Gelenler</h2>
                    <p class="lead mb-0">Vue hakkında yorumlar, yenilikler, gelişmeler</p>
                </div>
                <div class="row gx-5 justify-content-center">
                    <div v-for="post in posts" :key="post.id" class="col-lg-6">
                        <!-- deneme yazı-->
                       <SinglePost :post="post"/>
                    </div>
                </div>
            </div>
    </div>
</template>
<script>
import { ref } from "vue"
import GetPost from "../composables/GetPost";
import SinglePost from "../components/SinglePost.vue"
export default {
    name: "Post",
    components: { SinglePost },
    setup() {
    const posts = ref();
    GetPost().then((data) => {
      posts.value = data;
    });

    return  {posts} ;
    }
}
</script>
<style>
 .post{
    color: #fff;
}
   
    
</style>
<template>
    <div>
        <div class="container px-5 my-5 px-5">
                <div class="text-center mb-5">
                <h2 class="explain fw-bolder">Haydi Vue Blog'u geliştirmemize sen de yardımcı ol!</h2>
                <p class="explain lead mb-0">Yaz, gönder, yayınlayalım...</p>
                </div>
                <div class="row gx-5 justify-content-center">
                    <div class="col-lg-6">
                        
                        <form @submit.prevent="handleSubmit">
                            <div class="form-floating mb-3">
                                <input v-model="title" class="form-control" type="text" placeholder="Başlık girin..."/>
                                <label for="title">Başlık</label>
                            </div>
                            <!-- Nick Name input-->
                            <div class="form-floating mb-3">
                                 <input v-model="name" class="form-control" type="text" placeholder="Nick Name/ Takma İsim"/>
                                <label for="name">Nick Name/Takma İsim</label>
                            </div>
    
                            <!-- Message input-->
                            <div class="form-floating mb-3">
                                <textarea v-model="message" class="form-control" id="message" type="text" placeholder="Enter your message here..." style="height: 10rem"></textarea>
                                <label for="message">Mesaj</label>
                            </div>
                           
                            <!-- Submit Button-->
                            <div class="d-grid"><button class="buton btn btn-outline-dark btn-lg" type="submit">Gönder</button></div>
                        </form>
                    </div>
                </div>
            </div>
    </div>
</template>
<script>
import { ref } from 'vue';
import { fb } from '../firebase/config'
import { addDoc, collection, getFirestore } from 'firebase/firestore/lite';
import { useRouter } from 'vue-router'
 
export default {
    setup(){
        const title = ref();
        const name = ref();
        const message = ref();
        const router = useRouter()

        function handleSubmit(){
            const post = {
            title: title.value,
            name: name.value,
            message: message.value
        };
        const db = getFirestore(fb)
        const fbRef = collection(db,"posts")
        addDoc(fbRef, post)
        router.push({
            name: "Post"
        })
        }
       return {title, name, message, handleSubmit}
        
    }
 }
</script>

<style>
.buton{
  box-shadow: 0 12px 20px 0 #055f41, 0 6px 12px 0 #2387f9;
  color: #999
}
.buton:hover{
  color: #fff !important;
 }
 .explain{
    color: #999;
 }
</style>
<template>
    <div>
        <div class="container px-5 my-5 px-5">
                <div class="text-center mb-5">
                <h2 class="fw-bolder">Haydi Vue Blog'u geliştirmemize sen de yardımcı ol!</h2>
                <p class="lead mb-0">Yaz, gönder, yayınlayalım...</p>
                </div>
                <div class="row gx-5 justify-content-center">
                    <div class="col-lg-6">
                        
                        <form id="contactForm" >
                            <div class="form-floating mb-3">
                                <input class="form-control" id="title" type="text" placeholder="Başlık girin..."/>
                                <label for="title">Başlık</label>
                            </div>
                            <!-- Nick Name input-->
                            <div class="form-floating mb-3">
                                 <input class="form-control" id="name" type="text" placeholder="Nick Name/ Takma İsim"/>
                                <label for="name">Nick Name/Takma İsim</label>
                            </div>
    
                            <!-- Message input-->
                            <div class="form-floating mb-3">
                                <textarea class="form-control" id="message" type="text" placeholder="Enter your message here..." style="height: 10rem"></textarea>
                                <label for="message">Message</label>
                            </div>
                           
                            <!-- Submit Button-->
                            <div class="d-grid"><button class="btn btn-primary btn-lg disabled" id="submitButton" type="submit">Submit</button></div>
                        </form>
                    </div>
                </div>
            </div>
    </div>
</template>
<script>

</script>
<style>
    
</style>
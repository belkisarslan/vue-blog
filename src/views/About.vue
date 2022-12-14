<template>
  <div class="about">
    <header class="masthead text-center text-white">
            <div class="masthead-content">
                <div class="container px-5">
                    <h1 class="masthead-heading mb-0">Biz Kimiz?</h1>
                    <h2 class="masthead-subheading mb-0">Vue Hakkında söyleyecekleri olan bir grup çılgın</h2>
                </div>
            </div>

        </header>
        <section id="scroll">
            <div class="container px-5">
                <div class="row gx-5 align-items-center">
                    <div class="col-lg-6 order-lg-2">
                        <div class="p-5"><img class="img-fluid rounded-circle" src="https://i.pravatar.cc/300?img=48" alt="..." /></div>
                    </div>
                    <div class="col-lg-6 order-lg-1">
                        <div class="p-5">
                            <h2 class="display-4 style-text">Çılgın 1</h2>
                            <p class="style-text">Bence Vue.js kuzey ışıkları gibi; göz kamaştırıcı ve ihtişamlı.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <div class="container px-5">
                <div class="row gx-5 align-items-center">
                    <div class="col-lg-6">
                        <div class="p-5"><img class="img-fluid rounded-circle" src="https://i.pravatar.cc/300?img=68" alt="..." /></div>
                    </div>
                    <div class="col-lg-6">
                        <div class="p-5">
                            <h2 class="display-4 style-text">Çılgın 2</h2>
                            <p class="style-text">Bence Vue.js aslında yok. Hepsi bir ilizyon!</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <div class="container px-5">
                <div class="row gx-5 align-items-center">
                    <div class="col-lg-6 order-lg-2">
                        <div class="p-5"><img class="img-fluid rounded-circle" src="https://i.pravatar.cc/300?img=54" alt="..." /></div>
                    </div>
                    <div class="col-lg-6 order-lg-1">
                        <div class="p-5">
                            <h2 class="display-4 style-text">Çılgın 3</h2>
                            <p class="style-text">Bence Vue.js ...</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
  </div>
</template>
<style>
.style-text{
  color: #999;
}
header.masthead {
  position: relative;
  overflow: hidden;
  padding-top: 7rem;
  padding-bottom: 7rem;
  background: url("https://picsum.photos/id/901/1000/400");
  background-repeat: no-repeat;
  background-position: center center;
  background-attachment: scroll;
  background-size: cover;
}
header.masthead .masthead-content {
  z-index: 1;
  position: relative;
}
header.masthead .masthead-content .masthead-heading {
  font-size: 3rem;
}
header.masthead .masthead-content .masthead-subheading {
  font-size: 1rem;
}


</style>
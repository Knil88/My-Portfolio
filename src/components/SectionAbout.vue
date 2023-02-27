<script>
export default{
    data() {
        return {
            image:'data:image/png;base64,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'
        }
    },
}

</script>

<template>

<section class="container-fluid w-80 m-auto"   id="About">
    <div class="container col-xxl-8 px-4 py-5 " data-aos="fade-left">
        <div class="row flex-lg-row-reverse align-items-center g-5 py-5">
            <div class="col-10 col-sm-8 col-lg-6 m-auto d-flex justify-content-center">
                <img :src="image" class="d-block mx-lg-auto img-fluid align-" id='im_age' alt="logo Boolean" loading="lazy">
              </div>
          <div class="col-lg-6 text-center" data-aos="fade-right"  >
            <h1 class="display-5 fw-bold lh-1 mb-3 text-white">About Me</h1>
            <p class="paragrap_h" id="simpleUsage">

            </p>
          </div>
        </div>
      </div>

</section>
        
    
</template>

<style lang="scss">

    #About{
    padding-top: 15px;
}

.paragrap_h{
    color: #09d99a;
    border: 10px solid whitesmoke;
    background-color: black;
    font-family: 'Anonymous Pro', monospace;
    padding: 15px;
    min-height: 480px;
    font-size: 14px;
}

#im_age{
   min-width: 480px;
   padding-top: 20%; 
   min-height: 480px;
   
    
   
    
}

</style>
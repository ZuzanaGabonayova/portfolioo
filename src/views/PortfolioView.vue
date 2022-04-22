<template>
  
  <article id="portfolio">
            <div class="container-fluid portfolio">
                <h1 class="section-header">Portfolio</h1>

                <!-- <div class="row">
                  <div class="col-12 filter">
                    <button type="button" @click="categoryPhoto()" class="btn">PHOTOS</button>
                    <button type="button" @click="categoryIllustration()" class="btn">ILLUSTRATIONS</button>
                    <button type="button" @click="categoryPoster()" class="btn">POSTERS</button>
                    <button type="button" @click="categoryWeb()" class="btn ">WEBSITES</button>
                  </div>
                </div> -->


                <div  class="row photos"
                      data-aos="fade-up"
                      data-aos-duration="1000"
                >
                  <div class="col-sm-12 col-md-4 flex-col portfolio-item">
                    <img src="../assets/images/portfolio/photos/church.png" alt="church_photo" class="church_photo obr">
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Night photo of church with moon</h3>
                      </div>
                    </div> -->
                  </div>

                  <div class="col-sm-12 col-md-4 flex-col portfolio-item">
                    <img src="../assets/images/portfolio/photos/person.png" alt="person" class="person obr">
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Photo of girl looking into the sun</h3>
                      </div>
                    </div> -->
                  </div>

                  <div class="col-sm-12 col-md-4 flex-col portfolio-item">
                    <img src="../assets/images/portfolio/photos/sea.png" alt="sea" class="sea obr">
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Photo of sunset</h3>
                      </div>
                    </div> -->
                  </div>
                </div>


                <div  class="row illustrations"
                      data-aos="fade-up"
                      data-aos-duration="1000"
                >
                  <div class="col-sm-12 col-md-4 flex-col portfolio-item">
                    <img src="../assets/images/portfolio/illustrations/bear.png" alt="bear" class="bear obr">
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Illustration of bear</h3>
                      </div>
                    </div> -->
                  </div>

                  <div class="col-sm-12 col-md-4 flex-col portfolio-item">
                    <img src="../assets/images/portfolio/illustrations/trapholt-museum.png" alt="trapholt" class="trapholt obr">
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Trapholt museum illustration</h3>
                      </div>
                    </div> -->
                  </div>

                  <div class="col-sm-12 col-md-4 flex-col portfolio-item">
                    <img src="../assets/images/portfolio/posters/poster_halloween.png" alt="poster_halloween" class="poster_halloween obr">
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Halloween poster</h3>
                      </div>
                    </div> -->
                  </div>

                </div>


                <div  class="row websites"
                      data-aos="fade-up"
                      data-aos-duration="1000"
                >
                  <div class="col-sm-12 col-md-6 flex-col portfolio-item">
                    <video style="max-width:70%; max-height:auto display:block" autoplay loop muted>
                      <source src="../assets/images/portfolio/websites/apple_shop.mp4" type="video/mp4">
                    </video>
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Apple eshop - high school project</h3>
                      </div>
                    </div> -->
                  </div>

                  <div class="col-sm-12 col-md-6 flex-col portfolio-item">
                    <video style="max-width:70%; max-height:auto display:block" autoplay loop muted>
                      <source src="../assets/images/portfolio/websites/trapholt.mp4" type="video/mp4">
                    </video>
                    <!-- <div class="overlay">
                      <div class="portfolio-item-content">
                        <h3>Trapholt museum website - 1st semester exam project
                          <br>
                          https://trapholt.6f.sk/
                        </h3>
                      </div>
                    </div> -->
                  </div>

                </div>
              

            </div>
  </article>

</template>


<script>

export default {
  name: "PortfolioView"
}

</script>


<style lang="scss">
  
  $headings-color: #E3A905;
  $white-color: #ffffff;
  $black-color: #000000;
  $gray-color: #707070;


  *{
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}


#portfolio {
  height: 200vh!important;


  .photos,
  .illustrations,
  .websites{
    height: 60vh;
    min-height: fit-content;
    justify-content: center;
    align-items: center;

    .obr{
      height: 50vh;
    }
  }
}



/* .portfolio-item{

  
  .overlay {
    position: absolute;
    padding: inherit;
    top: 0;
    bottom: 0;
    width: 17.5vw;
    height: 50vh!important;
    opacity: 0;
    transition: 0.5s ease;
    background-color: #22222295;
    text-align: center;
    margin-left: 5.2vw;
    margin-top: 4.5vh;


    .portfolio-item-content {
      position: absolute;
      width: 100%;
      top: 0;
      bottom: 0;
      overflow: hidden;
      color: #ffffff;
      vertical-align: middle;
      text-align: center;
    }
  }




  &:hover .overlay {
    opacity: 0.95;
    cursor: pointer;
  }

  .overlay .portfolio-item-content {
    margin-top: 50%;
    overflow: hidden;
    color: $white-color;
    vertical-align: middle;
    text-align: center;
    h3 {
      font-size: 0.6rem;
      justify-content: center;
      align-items: center;
    }
  }
} */

      









@media only screen and (max-width: 990px){
  #portfolio {
  height: 325vh!important;

  .websites{
    height: 40vh;
  }

  .photos,
  .illustrations
  {
    height: 130vh;

    .obr{
      height: 35vh;
    }
  }
}
}



</style>
<template>
  
    
    <article id="about">
            <div class="container-fluid about">
                <h1 class="section-header">About</h1>

                <div class="row">
                    <div
                        class="col-sm-12 col-md-6 flex-col"
                        data-aos="fade-right"
                        data-aos-duration="1000"
                        style="margin: 0 auto;"
                    >
                        <p>
                            
                            <span id="bio">
                              My name is Zuzana! I am a creative and highly motivated multimedia designer with a strong background in programming, designing and UX/UI experiences. I mainly work with graphics, illustrations and websites, but I also have some experience in photo and videography.
                              <br>
                              <br>
                              I am constantly trying to find the middle ground between creativity and a logical mindset. I work well individually and in team, as well and I tend to bring a detail-oriented approach. I always work hard to achieve the best results and give customers the best product.
                            </span>
                        </p>


                        <!-- <h5>Here you can download my CV:
                            <a href="" download>
                                <img src="" alt="downloadCV" class="download">
                            </a>
                        </h5> -->

                        <div class="buttons-container">

                          <button class="contact" onclick="location.href = '#contact';">
                            CONTACT ME
                          </button>

                          <a href="../images/about/cv_zg.pdf" class="download-cv-zg" download="">
                            <button class="download">
                              DOWNLOAD CV
                            </button>
                          </a>

                        </div>

                    </div>

                    <div
                        class="col-sm-12 col-md-6 flex-col"
                        data-aos="fade-up"
                        data-aos-duration="1000"
                    >
                        <a href="https://drive.google.com/file/d/13LXiLVdhf2AMOvvJxBpjmv82jtRpS_eg/view?usp=sharing" target="_blank">
                            <img src="../assets/images/about/CV_frontpage.png" alt="cv" class="cv">
                        </a>

                    </div>

                </div>
            </div>
        </article>


        <div class="video-cv"
              data-aos="fade-up"
              data-aos-duration="1000"
        >
          <h5>Here you can watch my video CV :)</h5>
          <iframe width="560" height="315" src="https://www.youtube.com/embed/dFtEtHSeNj4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>

 
</template>



<script>

export default {
  name: "AboutView"
}

</script>



<style lang="scss" scoped>


$headings-color: #E3A905;
$white-color: #ffffff;
$black-color: #000000;
$gray-color: #707070;


/* *{
  font-family: 'Merriweather', serif;
} */

*{
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}




#about{
    min-height: 100vh;
    height: max-content;
    color: $white-color;

    .about p{
      font-size: 1rem;
      font-weight: normal;
      text-align: left;
      margin-top: 8%;
      padding-left: 15%;
    }

    .about .buttons-container{
      margin-top: 10%;
      text-align: left;
      padding-left: 15%;

      button {
        border: 2px solid $headings-color;
        padding: 10px 20px; 
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        border-radius: 20px;
      }


      .contact{
        font-weight: bold;
        background-color: $headings-color;
        color: $white-color;

        &:hover{
          background-color: #e3a80580;
        }
      }

      .download{
        margin-left: 30px;
        font-weight: bold;
        background-color: transparent;
        color: $headings-color;

        &:hover{
          background-color: #e3a80580;
        }
      }
    }

    .cv{
      height: 60vh;
      border: 3px solid $headings-color;
    }
}

.video-cv{
  height: 60vh;
  width: auto;
  min-height: 60vh;
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: column;
  
  iframe{
    border: 3px solid $headings-color;
  }
}


@media only screen and (max-width: 990px){
  #about{

    .about p{
      margin-top: 0%;
      padding-left: 0%;
    }


    .about .buttons-container{
      padding-left: 0%;
      justify-content: center;
      align-items: center;
      display: flex;
      flex-direction: column;
      gap: 15px;

      .download{
        margin-left: 0px;
      }
    }

    .cv{
      width: 70vw;
      height: auto;
    }
  }

  .video-cv{
    height: 40vh;
    min-height: 40vh;

    iframe{
      width: 70vw;
      height: auto;
    }
  }

  article .container-fluid{
    margin: 0rem!important;
  }
}

</style>
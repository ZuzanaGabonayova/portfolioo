<template>
  
  <article id="contact">
            <div class="container-fluid contact">
                <h1 class="section-header">Contact</h1>
                
                <div class="row">
                    <!-- start of "STAY IN TOUCH WITH ME" content  -->
                    <div
                        class="col-sm-12 col-md-6 flex-col"
                        data-aos="fade-right"
                        data-aos-duration="1000"
                        style="margin: 0 auto;"
                    >
                        <div class="contact-content">
                            <h2>STAY IN TOUCH WITH ME</h2>
                            <div class="contact-info">
                                <ul>
                                    
                                    <li class="location">
                                        <h3 class="d-inline">
                                            <i class="fas fa-map-marker-alt"></i>
                                        </h3>
                                        <br class="d-md-none" />
                                        <span>&nbsp; 6700 Esbjerg, Denmark</span>
                                    </li>

                                    <li class="phone">
                                        <h3 class="d-inline">
                                            <i class="fas fa-phone"></i>
                                        </h3>
                                        <br class="d-md-none" />
                                        <span class="sk">&nbsp; 
                                            <img src="../assets/images/flag-slovakia.png" alt="flag-slovakia" class="country-img">
                                            +421 950 797 735
                                        </span>
                                        <br>
                                        <span class="dk">&nbsp; 
                                            <img src="../assets/images/flag-denmark.png" alt="flag-denmark" class="country-img">
                                            +45 55 25 57 69
                                        </span>
                                    </li>

                                    <li class="email">
                                        <h3 class="d-inline">
                                            <i class="fas fa-envelope"></i>
                                        </h3>
                                        <br class="d-md-none" />
                                        <a href="mailto:gabonayova.zuzka@gmail.com">
                                            <span>&nbsp; gabonayova.zuzka@gmail.com</span>
                                        </a>
                                    </li>

                                    <li class="social">
                                        <h3 class="d-inline">
                                            <i class="fas fa-user-plus"></i>
                                        </h3>
                                        <br class="d-md-none" />
                                        
                                        <div class="social-item social-spacing list-inline-item">
                                            
                                                <a href="twitter.com" alt="twitter">
                                                    <i class="fab fa-twitter-square"></i>
                                                </a>
                                              
                                                <a href="https://www.facebook.com/zuzka.gabonayova" alt="facebook">
                                                    <i class="fab fa-facebook-square"></i>
                                                </a>
                                              
                                                <a href="https://github.com/ZuzanaGabonayova" alt="github">
                                                    <i class="fab fa-github-square"></i>
                                                </a>
                                              
                                                <a href="https://www.linkedin.com/in/zuzana-gabonayova/" alt="linkedin">
                                                    <i class="fab fa-linkedin"></i>
                                                </a>
                                              
                                                <a href="https://www.instagram.com/sjuzn36/" alt="instagram">
                                                    <i class="fab fa-instagram"></i>
                                                </a>
                                              
                                                <a href="snapchat.com" alt="snapchat">
                                                    <i class="fab fa-snapchat-square"></i>
                                                </a>
                                              
                                        </div>
                                    </li>

                                </ul>
                            </div>
                        </div>
                    </div>

                     <!-- end of "STAY IN TOUCH WITH ME" content  -->



                    <!-- start of contact form content  -->        
                    <div
                        class="col-sm-12 col-md-6 flex-col"
                        data-aos="fade-up"
                        data-aos-duration="1000"
                    >
                        <h2>SEND ME A MESSAGE</h2>

                        <div class="container contact-form">
                            <form action="https://app.99inbound.com/api/e/VOOJJSPy" method="POST" target="_blank">
                                <div class="form-group">
                                    <div class="input-group">
                                        <div class="input-group-prepend">
                                            <span class="input-group-text bg-white">
                                                <i class="fa fa-user"></i>&nbsp;
                                            </span>
                                        </div>
                                        <input name="name" type="name" placeholder="Name" class="form-control border-left-0" required>
                                    </div>
                                </div>

                                <div class="form-group">
                                    <div class="input-group">
                                        <div class="input-group-prepend">
                                            <span class="input-group-text bg-white">
                                                <i class="fa fa-envelope"></i>
                                            </span>
                                        </div>
                                        <input name="email" type="email" placeholder="E-mail" class="form-control border-left-0" required>
                                    </div>
                                </div>

                                <div class="form-group message">
                                    <div class="input-group">
                                        <div class="input-group-prepend">
                                            <span class="input-group-text bg-white">
                                                <i class="fas fa-comment-alt"></i>
                                            </span>
                                        </div>
                                        <textarea name="message" class="form-control" placeholder="Message..." id="message" rows="5"  required></textarea>
                                    </div>
                                </div>

                                <button type="submit" class="btn">
                                    <i class="fa fa-paper-plane"></i> 
                                    Send
                                </button>

                                <!-- Spam Prevention from 99inbound.com -->
                                <div style="position: absolute; left: -5000px;">
                                    <input type="checkbox" name="spectacular_cornflower_blue_plaid_chandelier" value="1" tabindex="-1" autocomplete="no">
                                </div>

                            </form>
                        </div>
                    </div>
                    <!-- end of contact form  -->
                </div>
            </div>
        </article>





</template>

<script>

export default {
  name: "ContactView"
}

</script>



<style lang="scss" scoped>

$headings-color: #E3A905;
$white-color: #ffffff;
$black-color: #000000;
$gray-color: #707070;




#contact {
  h2 {
    font-size: 1.4rem;
    font-weight: bold;
  }

  min-height: 100vh;
  height: max-content;
}

.contact .social-item {
  margin-left: 8%;

  a {
    text-decoration: none;
    color: $white-color;

    i:hover {
      color: $headings-color;
    }
  }

  i {
    font-size: 1.6rem;
    padding: 0 1rem;
  }
}

#contact .contact-content {
  ul {
    list-style-type: none;
    margin-top: 2rem;
  }

  .contact-info .location {
    justify-content: left;
  }
}

.country-img {
  width: 25px;
  height: auto;
}

.contact-info {
  font-size: 1rem;
  font-weight: 500;
  width: 90%;
  padding-left: 6%;

  ul {
    text-align: left;

    li {
      margin-top: 2.7rem;
      align-items: center;

      h3 {
        font-size: 1.3rem;
        color: $black-color;
      }
    }

    .location span {
      margin-left: 27.5%;
    }

    .phone {
      .sk {
        margin-left: 26.5%;
      }

      .dk {
        margin-left: 31.5%;
      }
    }

    .email a {
      text-decoration: none;
      color: $white-color;
      margin-left: 22%;

      &:hover {
        color: $headings-color;
      }
    }
  }
}

#contact .social-item {
  padding: 0 0.5rem;
}


/*contact form*/

  .btn,
  .btn-submit,
  .btn-success {
    background-color: $headings-color;
    border-color: transparent;
  }
  .btn:hover,
  .btn-submit:hover,
  .btn-success:hover {
    background-color: #e3a80580;
    color: #ffffff;
  }
  .contact-form {
    margin-top: 2rem;
  }
  .contact-form button {
    width: 100%;
  }

.contact-form{
    display: flex;
    justify-content: center;
    align-items: center;
}
form{
    width: 90%;
}
.contact-form .fa, .contact-form .fas{
    color: $black-color;
}
.contact-form ::placeholder{
    color: $gray-color;
    font-weight: 500;
}
button .fa{
    padding-right: 10px;
}
.btn{
    border-radius: 15px!important;
    font-weight: 500;
    color: $white-color;
}
textarea, input{
    border-top-right-radius: 15px!important;
    border-bottom-right-radius: 15px!important;
}
.input-group-text{
    border-top-left-radius: 15px!important;
    border-bottom-left-radius: 15px!important;
}
.input-group-text i{
    font-size: larger;
}
.btn i{
    font-size: larger;
}
textarea{
    border-left: 0px solid $white-color!important;
}
.message .input-group-text{
    border-right: $white-color;
    display: flex;
    align-items: flex-start;
}
.message .input-group-text i{
    padding-top: 6px;
}
.btn .fa{
    color: $white-color;
}

@media only screen and (max-width: 990px){
  .contact-info{
        padding: 0;
        align-items: center;
        justify-content: center;
        width: 100%;
    }
    .contact-info ul{
        padding-left: 0;
        text-align: center;
    }
    .contact .social-item{
        margin: 0;
    }
    .contact-info ul .location span{
        margin-left: 0;
    }
    .contact-info ul .phone .sk{
        margin-left: 0;
    }
    .contact-info ul .phone .dk{
        margin-left: 0;
    }
    .contact-info ul .email a{
        margin-left: 0;
    }
    .contact .social-item i {
        font-size: 1.6rem;
        padding: 0 1.4rem;
    }

    form{
        width: 100%;
    }

    .contact .social-item i{
        padding: 0.3rem;
    }
      
}


</style>
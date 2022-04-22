<template>

        <header>

          <nav class="navbar navbar-expand-lg fixed-top">
              <a href="#" class="navbar-brand">
                <div><img src="../assets/logo.png" alt="logo" id="logo"></div>
              </a>

              <button
                class="navbar-toggler"
                type="button"
                data-toggle="collapse"
                data-target="#navbarNavAltMarkup"
                aria-controls="navbarNavAltMarkup"
                aria-expanded="false"
                aria-label="Toggle navigation"
            >
                <span class="navbar-toggler-icon"><i class="fas fa-bars" style="color:#fff; font-size:28px;"></i></span>
            </button>
            <div id="navbarNavAltMarkup" class="collapse navbar-collapse">
                <ul id="navbar-nav" class="navbar-nav ml-auto">
                    <li class="active-nav">
                        <a class="nav-item nav-link" href="#">Home</a>
                    </li>
                    <li><a class="nav-item nav-link" href="#about">About</a></li>
                    <li><a class="nav-item nav-link" href="#skills">Skills</a></li>
                    <li><a class="nav-item nav-link" href="#portfolio">Portfolio</a></li>
                    <li><a class="nav-item nav-link" href="#contact">Contact</a></li>
                </ul>
            </div>
          </nav>
          
          

            <div class="hero-img-bg"></div>
          
            <div class="hero-text">
                <h1>ZUZANA GABONAYOVÁ</h1>
                
                <h3>
                    <span class="typed-text">{{ typeValue }}</span> 
                    <span class="cursor" :class="{'typing': typeStatus}">&nbsp;</span>
                </h3>
            </div>

          
        </header>



</template>


<script>

  export default {
    name: "HomeView",
    data: () => {
      return {
        typeValue: '',
        typeStatus: false,
        typeArray: ["Multimedia designer", "Web developer", "Graphic designer", "UX/UI designer"],
        typingSpeed: 200,
        erasingSpeed: 100,
        newTextDelay: 2000,
        typeArrayIndex: 0,
        charIndex: 0
      }
    },
    methods: {
      typeText() {
        if(this.charIndex < this.typeArray[this.typeArrayIndex].length) {
          if(!this.typeStatus)
            this.typeStatus = true;
          this.typeValue += this.typeArray[this.typeArrayIndex].charAt(this.charIndex);
          this.charIndex += 1;
          setTimeout(this.typeText, this.typingSpeed);
        }
        else {
          this.typeStatus = false;
          setTimeout(this.eraseText, this.newTextDelay);
        }
      },
      eraseText() {
        if(this.charIndex > 0) {
          if(!this.typeStatus)
            this.typeStatus = true;
          this.typeValue = this.typeArray[this.typeArrayIndex].substring(0, this.charIndex - 1);
          this.charIndex -= 1;
          setTimeout(this.eraseText, this.erasingSpeed);
        }
        else {
          this.typeStatus = false;
          this.typeArrayIndex += 1;
          if(this.typeArrayIndex >= this.typeArray.length)
            this.typeArrayIndex = 0;
          setTimeout(this.typeText, this.typingSpeed + 1000);
        }
      }
    },
    created() {
      setTimeout(this.typeText, this.newTextDelay + 200);
    }
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



body{
    height: 100%;
    margin: 0;
    padding: 0;
    color: $white-color;
}

header{
    height: 100vh;

    nav{
    background-color: #000000c8;
    height: 80px;

        ul li a{
        color: $white-color!important;
        text-decoration: none;

            

            &:hover{
                color: #e3a80580!important;
            }
            
        }

        .navbar-brand{
            margin-left: 50px;

            #logo {
                max-height: 4rem;
            }
        }


        #navbar-nav{
            margin-right: 5%;
            text-transform: uppercase;
            font-weight: bold;
            font-size: 14px;
            gap: 15px;
        }

        .active-nav a{
            color: $headings-color!important;
            font-weight: bolder;
        } 
        
    }

    .hero-img-bg {
        background-image: linear-gradient(to left bottom, #000000b1, #4e4e4eb3),url("../assets/images/mockup.png");
        height: 100vh;
        width: 100%;
        background-repeat: no-repeat;
        background-position: center center;
        background-size: cover;
        -webkit-background-size: cover;
        position: absolute;
    }  

    .hero-text{
        display: inline-block;
        vertical-align: middle;
        margin: auto;
        width: 85%;
        padding-bottom: 2rem;
        text-align: center;
        position: absolute;
        top: 50%;
        left: 50%;
            -webkit-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
        font-weight: bold;
        color: $white-color;



        h1{
            font-size: 4rem;
            font-weight: bolder;
            text-transform: uppercase;
        }

        h3{
            padding-top: 4%;
            font-size: 2.5rem;
            font-weight: bold;

            span.typed-text {
                color: $white-color;
            }

            span.cursor {
                display: inline-block;
                margin-left: 3px;
                width: 4px;
                background-color: $white-color;
                animation: cursorBlink 1s infinite;
            }

            span.cursor.typing {
                animation: none;
            }
        }
    }
}


@keyframes cursorBlink {
  49% { background-color: #fff; }
  50% { background-color: transparent; }
  99% { background-color: transparent; }
}


@media only screen and (max-width: 990px){
    header{

        nav{
            height: auto;
            background-color: $black-color;
            

            .navbar-nav{
                align-items: center;
                margin-right: 0!important;
            }
            
            .navbar-brand{
                margin-left: 0px;
            }
        }

        .hero-text{

            h1 {
                margin-top: 0%;
                font-size: 2.7rem;
            }

            h3{
                margin-top: 20%;
                font-size: 1.5rem;
            }
        }
    }
     
}

</style>


<template>

  <footer class="footer font-small text-center">
    
            <ul class="list-inline">
              <li class="social-item list-inline-item">
                <a href="https://twitter.com/" alt="twitter">
                    <i class="fab fa-twitter-square"></i>
                </a>
              </li>
              <li class="social-item list-inline-item">
                <a href="https://www.facebook.com/zuzka.gabonayova" alt="facebook">
                    <i class="fab fa-facebook-square"></i>
                </a>
              </li>
              <li class="social-item list-inline-item">
                <a href="https://github.com/ZuzanaGabonayova" alt="github">
                    <i class="fab fa-github-square"></i>
                </a>
              </li>
              <li class="social-item list-inline-item">
                <a href="https://www.linkedin.com/in/zuzana-gabonayova/" alt="linkedin">
                    <i class="fab fa-linkedin"></i>
                </a>
              </li>
              <li class="social-item list-inline-item">
                <a href="https://www.instagram.com/sjuzn36/" alt="instagram">
                    <i class="fab fa-instagram"></i>
                </a>
              </li>
              <li class="social-item list-inline-item">
                <a href="https://snapchat.com" alt="snapchat">
                    <i class="fab fa-snapchat-square"></i>
                </a>
              </li>
            </ul>
        
            <div class="copyright">
              <p>
                Copyright © 2022 Zuzana Gabonayová. All Rights Reserved.
              </p>
            </div>
            
          </footer>

</template>





<script>

export default {
  name: "FooterView"
}

</script>


<style lang="scss">


$headings-color: #E3A905;
$white-color: #ffffff;
$black-color: #000000;
$gray-color: #707070;


footer {
  margin-top: 5%;
  height: 20vh;
  font-size: 0.7rem;
  padding: 1rem;
}

.footer {
  a {
    text-decoration: none;
    color: $white-color;

    i:hover {
      color: $headings-color;
    }
  }

  .social-item i {
    font-size: 1.9rem;
    padding: 0 2rem;
  }

  .copyright {
    margin-top: 2%;
    font-weight: 500;
  }
}


@media only screen and (max-width: 990px){
    .footer .social-item i{
        padding: 0rem;
    }
}

</style>
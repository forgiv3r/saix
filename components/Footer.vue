<template>
  <div>
    <footer class="footer_1">
    <div class="container">
      <div class="row">
        <div class="col-lg-5 col-sm-6 col-md-5">
          <aside class="widget aboutwidget">
            <a href="#"><img src="/images/foo_logo.png" alt=""></a>
            <p>
              Dzargo is a men's fashion brand that was founded in a small village in Purbalingga Regency since 2020. We are here full of enthusiasm with the goal of promoting local Indonesian brands.
            </p>
          </aside>
        </div>
        <div class="col-lg-4 col-sm-4 col-md-4">
          <aside class="widget contact_widgets">
            <h3 class="widget_title">contact</h3>
            <p>
              Address:<br>
              Jl. Raya Majingklak, Karangmoncol<br>
              Purbalingga 53355
            </p>
            <p>Phone: (0281) 7700761</p>
            <p>Email:<a href="#">hi@dzargo.id</a></p>
          </aside>
        </div>
        <div class="col-lg-3 col-sm-2 col-md-3">
          <aside class="widget social_widget">
            <h3 class="widget_title">social</h3>
            <ul>
              <li><a href="https://instagram.com/dzargoid"><i></i>Instagram</a></li>
              <li><a href="https://www.facebook.com/dzargooo"><i></i>Facebook</a></li>
              <li><a href="https://www.linkedin.com/company/dzargoindonesia/"><i></i>Linkedin</a></li>
            </ul>
          </aside>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12 col-sm-12 text-center">
          <div class="copyright">
            © copyright 2021 <a href="#">Dzargo</a>.
            <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0</a>
          </div>
        </div>
      </div>
    </div>
  </footer>

    <!-- Bact To To -->
    <a id="backToTop" href="#" class=""><i class="fa fa-angle-double-up"></i></a>
    <!-- Bact To To -->


  </div>
</template>

<script>
    export default {
      name: "Footer",
      mounted() {

        var back = $("#backToTop"),
          body = $("body, html");
        $(window).on('scroll', function () {
          var h = $(window).height() / 2;
          if ($(window).scrollTop() > h)
          {
            back.addClass('showit');
          } else
          {
            back.removeClass('showit');
          }

        });
        body.on("click", "#backToTop", function (e) {
          e.preventDefault();
          body.animate({scrollTop: 0}, 800);
        });

      }
    }
</script>

<style scoped>

</style>

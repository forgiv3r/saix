<template>
  <section class="commonSection team">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="sec_title">- Our Family -</h2>
        </div>
      </div>
    </div>
    <div class="team_slider">
      <div class="singleTM">
        <div class="tm_img">
          <img src="/images/team/1.jpg" alt="">
          <div class="tm_overlay">
            <div class="team_social">
              <a href="https://www.instagram.com/ctr_all/"><span></span></a>
            </div>
            <a class="common_btn"><span>@ctr_all</span></a>
          </div>
        </div>
        <div class="detail_TM">
          <h5>Catur Kurnia Putra</h5>
          <h6>Founder & CEO</h6>
        </div>
      </div>
      <div class="singleTM">
        <div class="tm_img">
          <img src="/images/team/2.jpg" alt="">
          <div class="tm_overlay">
            <div class="team_social">
              <a href="#"><span>Instagram</span></a>
            </div>
            <a class="common_btn"><span>@deacnsulistio</span></a>
          </div>
        </div>
        <div class="detail_TM">
          <h5>Dea Cici N</h5>
          <h6>Dept Head HRD</h6>
        </div>
      </div>
      <div class="singleTM">
        <div class="tm_img">
          <img src="/images/team/3.jpg" alt="">
          <div class="tm_overlay">
            <div class="team_social">
              <a href="#"><span>Instagram</span></a>
            </div>
            <a href="#" class="common_btn"><span>tentang</span></a>
          </div>
        </div>
        <div class="detail_TM">
          <h5>Putri Tri M</h5>
          <h6>Dept Head FAT</h6>
        </div>
      </div>
      <div class="singleTM">
        <div class="tm_img">
          <img src="/images/team/4.jpg" alt="">
          <div class="tm_overlay">
            <div class="team_social">
            </div>
            <a class="common_btn"><span>@anggydsw</span></a>
          </div>
        </div>
        <div class="detail_TM">
          <h5>Anggy Dwi Setyo W</h5>
          <h6>Dept Head Sales Marketing</h6>
        </div>
      </div>
      <div class="singleTM">
        <div class="tm_img">
          <img src="/images/team/5.jpg" alt="">
          <div class="tm_overlay">
            <div class="team_social">
            </div>
            <a class="common_btn"><span>@odisusanto</span></a>
          </div>
        </div>
        <div class="detail_TM">
          <h5>Odi Susanto</h5>
          <h6>General Affair</h6>
        </div>
      </div>
      <div class="singleTM">
        <div class="tm_img">
          <img src="/images/team/6.jpg" alt="">
          <div class="tm_overlay">
            <div class="team_social">
            </div>
            <a href="https://www.linkedin.com/in/odi-susanto-66b42512b/" class="common_btn"><span>@lukikhoerul</span></a>
          </div>
        </div>
        <div class="detail_TM">
          <h5>Luki Khoerul</h5>
          <h6>Head of Production</h6>
        </div>
      </div>

    </div>
  </section>
</template>

<script>
    export default {
      name: "Team",
      mounted() {
        if ($('.team_slider').length > 0) {
          $('.team_slider').slick({
            autoplay: true,
            autoplaySpeed: 2000,
            slidesToShow: 3,
            dots: true,
            arrows: false,
            centerMode: true,
            centerPadding: '350px',
            responsive: [
              {
                breakpoint: 1600,
                settings: {
                  centerMode: true,
                  centerPadding: '40px',
                  slidesToShow: 4
                }
              },
              {
                breakpoint: 1199,
                settings: {
                  centerMode: true,
                  centerPadding: '40px',
                  slidesToShow: 3
                }
              },
              {
                breakpoint: 991,
                settings: {
                  centerMode: true,
                  centerPadding: '40px',
                  slidesToShow: 2
                }
              },
              {
                breakpoint: 600,
                settings: {
                  centerMode: true,
                  centerPadding: '30px',
                  slidesToShow: 1
                }
              }
            ]
          });
        }
      }
    }
</script>

<style scoped>

</style>

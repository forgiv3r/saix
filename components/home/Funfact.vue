<template>
    <div>
      <section class="commonSection funfact">
        <div class="container">
          <div class="row">
            <div class="col-lg-3 col-sm-6 col-md-3 noPadding BR">
              <div class="singlefunfact text-center">
                <h1 data-counter="20350" class="timer"><span class="countSpan">20</span>350</h1>
                <h3>Sales</h3>
              </div>
            </div>
            <div class="col-lg-3 col-sm-6 col-md-3 noPadding BR">
              <div class="singlefunfact text-center">
                <h1 data-counter="11780" class="timer"><span class="countSpan"></span>11780</h1>
                <h3>Happy Customers</h3>
              </div>
            </div>
            <div class="col-lg-3 col-sm-6 col-md-3 noPadding BR">
              <div class="singlefunfact text-center">
                <h1 data-counter="53" class="timer"><span class="countSpan"></span>53</h1>
                <h3>Collaboration</h3>
              </div>
            </div>
            <div class="col-lg-3 col-sm-6 col-md-3 noPadding">
              <div class="singlefunfact text-center">
                <h1 data-counter="2" class="timer"><span class="countSpan"></span>2</h1>
                <h3>Years Working</h3>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
</template>

<script>
    export default {
      name: "Funfact",
      mounted() {
        var skl = true;
        $('.singlefunfact').appear();
        $('.singlefunfact').on('appear', function () {
          if (skl)
          {
            $('.timer').each(function () {
              var $this = $(this);
              jQuery({Counter: 0}).animate({Counter: $this.attr('data-counter')}, {
                duration: 3000,
                easing: 'swing',
                step: function () {
                  var num = Math.ceil(this.Counter).toString();
                  if (Number(num) > 999) {
                    while (/(\d+)(\d{3})/.test(num)) {
                      num = num.replace(/(\d+)(\d{3})/, '<span class="countSpan">' + '$1' + '</span>' + '$2');
                    }
                  }
                  $this.html(num);
                }
              });
            });
            skl = false;
          }
        });
      }
    }
</script>

<style scoped>

</style>

<template>
  <div>
    <SliderOne />
    <Services />
    <AboutDzargo />
    <WhatWeDo />
    <Funfact />
    <Portfolio />
    <Team />
    <CallToAction />
    <Patner />
  </div>
</template>

<script>
  import SliderOne from "~/components/home/SliderOne";
  import Services from "~/components/home/Services";
  import AboutDzargo from "~/components/home/AboutDzargo";
  import WhatWeDo from "~/components/home/WhatWeDo";
  import Funfact from "~/components/home/Funfact";
  import Portfolio from "~/components/home/Portfolio";
  import Team from "~/components/home/Team";
  import CallToAction from "~/components/home/CallToAction";
  import Patner from "~/components/home/Patner";
  export default {
    components: {
      SliderOne,
      Services,
      AboutDzargo,
      WhatWeDo,
      Funfact,
      Portfolio,
      Team,
      CallToAction,
      Patner,


    }
  }
</script>

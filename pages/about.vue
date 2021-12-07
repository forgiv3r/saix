<template>
  <div>
    <PageBanner pageTitle="About Us" />
    <AboutDzargo />
    <Team />
    <Patner />
  </div>
</template>
<script>
  import PageBanner from "~/components/pages/PageBanner";
  import AboutDzargo from "~/components/home/AboutDzargo";
  import Team from "~/components/home/Team";
  import Patner from "~/components/home/Patner";
  export default {
    components: {
      PageBanner,
      AboutDzargo,
      Team,
      Patner
    },
    head(){
      return {
        title: "Dzargo | About Us"
      }
    }
  }
</script>

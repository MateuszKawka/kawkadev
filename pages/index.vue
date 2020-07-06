<template>
  <div>
    <Navigation />
    <Header />
    <Exp />
    <Works />
    <Skills />
  </div>
</template>
<script>
import Header from "~/components/sections/Header";
import Navigation from "~/components/Navigation";
import Exp from "~/components/sections/Exp";
import Works from "~/components/sections/Works"
import Skills from "~/components/sections/Skills"
export default {
  name: "HomePage",
  components: {
    Header,
    Navigation,
    Exp,
    Works,
    Skills
  }
};
</script>
<template>
  <div>
    <Nav />
    <Banner />
    <Service />
    <Brand />
    <Courses />
    <About />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Nav from "../components/Nav";
import Banner from "../components/Banner";
import Footer from "../components/Footer";
import Service from "../components/Service";
import About from "../components/About";
import Brand from "../components/Brand";
import Courses from "../components/Courses";
import Contact from "../components/Contact";

export default {
  components: {
    About,
    Contact,
    Courses,
    Brand,
    Service,
    Footer,
    Banner,
    Nav,
  },
};
</script>

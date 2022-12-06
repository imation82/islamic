<template>
  <div>
    <Map/>
    <Footer/>
    <FooterBottom/>
  </div>
</template>

<script>

import Map from '~/components/Map';
import Footer from '~/components/Footer';
import FooterBottom from '~/components/FooterBottom';

export default {
  name: 'Index',
  components: {
    Map,
    Footer,
    FooterBottom
  }
}
</script>
<template>
  <div>
    <Newsletter/>
    <StayInTouch/>
    <Map/>
    <Footer/>
    <FooterBottom/>
  </div>
</template>

<script>

import Newsletter from '~/components/Newsletter';
import StayInTouch from '~/components/StayInTouch';
import Map from '~/components/Map';
import Footer from '~/components/Footer';
import FooterBottom from '~/components/FooterBottom';

export default {
  name: 'Index',
  components: {
    Newsletter,
    StayInTouch,
    Map,
    Footer,
    FooterBottom
  }
}
</script>
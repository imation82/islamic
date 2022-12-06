<template>
  <div>
    <Khateebs/>
    <Newsletter/>
    <StayInTouch/>
    <Map/>
    <Footer/>
    <FooterBottom/>
  </div>
</template>

<script>

import Khateebs from '~/components/Khateebs';
import Newsletter from '~/components/Newsletter';
import StayInTouch from '~/components/StayInTouch';
import Map from '~/components/Map';
import Footer from '~/components/Footer';
import FooterBottom from '~/components/FooterBottom';

export default {
  name: 'Index',
  components: {
    Khateebs,
    Newsletter,
    StayInTouch,
    Map,
    Footer,
    FooterBottom
  }
}
</script>
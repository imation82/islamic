<template>
  <div>
    <Footer/>
    <FooterBottom/>
  </div>
</template>

<script>

import Footer from '~/components/Footer';
import FooterBottom from '~/components/FooterBottom';

export default {
  name: 'Index',
  components: {
    Footer,
    FooterBottom
  }
}
</script>
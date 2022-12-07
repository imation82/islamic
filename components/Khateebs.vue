
<template>
    <section class="khateebs">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <h2 class="text-center mb-4">Our Jummah Khateeb's</h2>
                </div>                
            </div>
            <div class="row mt-3">
                <div class="col-lg-10 offset-lg-1">
                    <div class="row">
                        <div class="col-lg-4" v-for="khateeb in khateebs" :key="khateeb.id">
                            <div class="khateebs__block mb-3 mb-lg-0">
                                <img src="" alt="Omar Ockeh" class="img-fluid d-block mx-auto">
                                <div class="khateebs__name">
                                    <h3>{{ khateeb.attributes.name }}</h3>
                                    <span class="khateebs__line"></span>
                                </div>
                            </div>
                        </div>
                        <!-- <div class="col-lg-4">
                            <div class="khateebs__block mb-3 mb-lg-0">
                                <img src="~assets/images/nabil_omran.jpg" alt="Nabil Omran" class="img-fluid d-block mx-auto">
                                <div class="khateebs__name">
                                    <h3>Sh. Dr. Nabil Omran</h3>
                                    <span class="khateebs__line"></span>
                                </div>
                            </div>                    
                        </div>
                        <div class="col-lg-4">
                            <div class="khateebs__block mb-3 mb-lg-0">
                                <img src="~assets/images/imam_shafeeq.jpg" alt="Imam Shafeeq" class="img-fluid d-block mx-auto">
                                <div class="khateebs__name">
                                    <h3>Sh. Dr. Imam Shafeeq</h3>
                                    <span class="khateebs__line"></span>
                                </div>
                            </div>                     
                        </div>                          -->
                    </div>
                </div>                               
            </div>            
        </div>
    </section>
</template>

<script>

import axios from 'axios'

export default {
  data () {
    return {
      khateebs: [],
    }
  },
  async mounted () {
      const response = await axios.get('http://localhost:1337/api/khateebs')
      this.khateebs = response.data.data
    } 
}

</script>
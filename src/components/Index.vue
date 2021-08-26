<template>
  <div>
    <Navbar />
    <Banner />
    <Content />
    <Button :height="innerHeigh" class="d-block d-md-none" />
    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Banner from '@/components/Banner.vue'
import Content from '@/components/Content.vue'
import Button from '@/components/Button.vue'
import Footer from '@/components/Footer.vue'
export default {
  data () {
    return {
      innerHeigh: ''
    }
  },
  components: {
    Navbar,
    Banner,
    Content,
    Footer,
    Button
  },
  methods: {
    handleScroll () {
      this.innerHeigh = window.scrollY
    }
  },
  mounted () {
    window.addEventListener('scroll', this.handleScroll, false)
  },
}
</script>

<template>
  <div class="scrollBtn"><a v-on:click.prevent="scrollTop" href="#top">TOP</a></div>
</template>

<script>
  import $ from 'jquery'

  export default {
    name: 'scrollTop',
    methods: {
      scrollTop: function () {
        $('a[href^="#"]').click(function () {
          var href = $(this).attr('href')
          var target = $(href === '#' || href === '' ? 'html' : href)
          var position = target.offset().top
          $('html,body').animate({scrollTop: position}, 500)
        })
      }
    }
  }
</script>

<style scoped>
.scrollBtn{
  display: block;
  height: 50px;
  width: 50px;
  position: fixed;
  bottom: 0;
}
</style>

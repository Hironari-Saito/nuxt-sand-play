<template>
  <section class="section-jquery">
    <ul class="section-jquery__startup flex">
      <li>
        <div class="square"></div>
      </li>
      <li>
        <div class="square"></div>
      </li>
      <li>
        <div id="circle">
          <p>override p tag</p>
        </div>
      </li>
    </ul>
    <div class="section-jquery__fade flex">
      <div class="square"></div>
      <div class="square"></div>
      <div class="square"></div>
    </div>
    <div class="section-jquery__animation flex">
      <div class="square"></div>
    </div>
  </section>
</template>
<script>
export default {
  mounted() {
    jQuery('.section-jquery__startup #circle').click(() => {
      $('#circle p').html('Over rided :)')
      // eslint-disable-next-line no-console
      console.log($('p').html())
    })

    $('.section-jquery__startup .square').hover(
      // hover in
      function () {
        $(this).css('background-color', 'rgba(100,99,100,0.4)')
      },
      // hover out
      function () {
        $(this).css('background-color', 'rgba(255,99,255,0.3')
        console.log($('.square').css('background-color'))
      }
    )
    $('.section-jquery__fade .square').hover(
      function () {
        $(this).fadeOut(1000)
      },
      function () {
        $(this).fadeIn(1000)
      }
    )
    $('.section-jquery__animation .square').click(function () {
      $(this).animate(
        {
          width: '400px',
          height: '300px',
          marginLeft: '150px',
        },
        300,
        function () {
          console.log('test')
          $(this).css('background-color', 'rgba(255,99,255,1')
        }
      )
    })
  },
}
</script>

<style lang="stylus" src="./index.stylus" scoped />

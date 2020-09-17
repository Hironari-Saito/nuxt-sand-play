<template>
  <div class="container mx-auto w-full max-w-screen-lg">
    <h1>Hover</h1>
    <section>
      <div>
        <h2>refer to http://kylebrumm.com</h2>
        <span
          >https://gist.github.com/kirishigure/8b7511e7dc9a957a48fa61efee3955af</span
        >
        <span>Kyle Brumm</span>
      </div>
      <div class="">
        <div class="design-display">
          <button class="flex-item btn btn--swipe">Swipe</button>
          <button class="flex-item btn btn--sharp-swipe">Sharp Swipe</button>
          <button class="flex-item btn btn--2sharp-swipe">Double Swipe</button>
          <button class="flex-item btn btn--diagonal-close">
            Diagonal Close
          </button>
          <button class="flex-item btn btn--zoning">Zoning</button>
          <button class="flex-item btn btn--4corners">
            <span class="btn--4corners-fragments">4 corners</span>
          </button>
          <button class="flex-item btn btn--slice">slice</button>
          <Position />
          <Alternate />
          <UpdownSlide />
          <VerticalOverlap />
        </div>
        <div class="wrap">
          <a class="btn-8" href="#">Smoosh</a>
          <a class="btn-9" href="#"><span>Vertical Overlap</span></a>
          <a class="btn-10" href="#"><span>Horizontal Overlap</span></a>
          <a class="btn-11" href="#">Collision</a>
        </div>
      </div>
    </section>
    <hr />
    <section>
      <h2>https://ianlunn.github.io/Hover/</h2>
    </section>
  </div>
</template>

<style lang="stylus" src="./index.stylus" scoped />

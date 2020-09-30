<template>
  <section class="section-jquery-ajax">
    <button @click="getInfoFile">GET info text</button>
    <p>override text here</p>
  </section>
</template>
<script>
export default {
  mounted() {
    // $.get('/info.txt', function (data) {
    //   alert(data)
    // })

    // Regex
    const regex = /Is/i
    const string = 'Regex is great'
    const result = string.match(regex)
    console.log(result)
  },
  methods: {
    getInfoFile() {
      $.ajax('/info.txt')
        .done(function (data) {
          $('.section-jquery-ajax p').html(data)
        })
        .fail(function (error) {
          $('.section-jquery-ajax p').html(error.status)
        })
    },
  },
}
</script>

<style lang="stylus" src="./index.stylus" scoped />

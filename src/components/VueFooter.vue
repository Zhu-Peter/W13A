<template>
  <footer>
    <section id="footer_social">
      <a href="">Facebook</a>
      <a href="">Twitter</a>
      <a href="">Myspace</a>
      <a href="">TikTok</a>
    </section>
    <section id="footer_legal">
      <a href="">Private Policy</a>
      <a href="">Newsletter</a>
    </section>
  </footer>
</template>

<script>
export default {
  name: 'VueFooter',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
footer {
  background-color: black;
  color: white;
  padding: 30px;
  padding-inline: 20px;
  display: grid;


  grid-template-columns: 1fr 1fr;
  align-items: start;
  justify-items: center;


  min-width: 65vw;
  margin-top: 4%;

  a {
    text-decoration: none;
    color: inherit;
  }

  >section {
    display: grid;
    align-items: start;
    line-height: 2;
    margin-inline: auto;
  }
}
</style>
<template>
  <div class="VueBody">
    <h1 id="title">Title</h1>
    <div id="num_friends"></div>
  </div>
</template>

<script>
export default {
  name: 'VueBody',
  props: {
    msg: String
  },
  data: function () {
    return {
      tweets: ['aaaaaa', 'bbbbbbc', 'ccccccc'],
      num_friends: 13,
      logged_in: true
    }
  },
  methods: {
    showInfo: function () {
      document.getElementById(`num_friends`).insertAdjacentHTML(`beforeend`, `<span>number of friends: ${this.num_friends}</span>`)
      if (this.logged_in) {
        document.getElementById(`num_friends`).insertAdjacentHTML(`beforeend`, `<h1>logged in</h1>`)
      } else { return }
      for (let i = 0; i < this.tweets.length; i++) {
        document.getElementById(`num_friends`).insertAdjacentHTML(`beforeend`, `<p>${this.tweets[i]}</p>`);
      }
      // console.log(this.num_friends)
    }
  },
  mounted() {
    this.showInfo();

  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.VueBody {
  box-sizing: border-box;
  background-color: aquamarine;
  width: 1400px;
  margin-inline: auto;
  padding: 50px;
}
</style>
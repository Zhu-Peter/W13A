<template>
  <div class="VueHeader">
    <div class="page_header_layout">
      <div class="page_header_logo">
        <img id="page_header_logo" src="../assets/logo.png" alt="logo" />
      </div>
      <nav class="page_header_menu">
        <svg class="page_header_menu_icon" version="1.1" id="menu_icon" viewBox="0 0 16 16" x="0px" y="0px"
          xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg">
          <g>
            <rect y="1" width="16" height="2"></rect>
            <rect y="7" width="16" height="2"></rect>
            <rect y="13" width="16" height="2"></rect>
          </g>
        </svg>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: 'VueHeader',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.page_header {
  display: block;
}

.page_header_layout {
  display: flex;
  flex-direction: column;
  align-items: start;
  min-height: 80px;
  width: 1200px;
  margin: 0 auto;
}

#page_header_logo {
  width: 100px;
  margin: 22px auto 0 0;
}

nav {
  width: auto;
  margin: -32px 0 22px auto;
}

#menu_icon {
  fill: orange;
  height: 2em;
  min-width: auto;
}

#menu_icon:hover{
  cursor: pointer;
}
</style>
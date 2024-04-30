<template>
    <div class="VueHeader">
        <div class="page_header_layout">
        <div class="page_header_logo">
          <img id="page_header_logo" src="images/default-logo.png" alt="logo" />
        </div>
        <nav class="page_header_menu">
          <svg
            class="page_header_menu_icon"
            version="1.1"
            id="menu_icon"
            viewBox="0 0 16 16"
            x="0px"
            y="0px"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            xmlns="http://www.w3.org/2000/svg"
          >
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

  </style>
  
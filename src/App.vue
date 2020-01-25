<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
  @font-face {
    font-family: 'AriaMT';
    src: url('assets/fonts/AriaMT.eot');
    src: local('☺'), url('assets/fonts/AriaMT.woff') format('woff'), url('assets/fonts/AriaMT.ttf') format('truetype'), url('assets/fonts/AriaMT.svg') format('svg');
    font-weight: normal;
    font-style: normal;
  }
  @font-face {
    font-family: 'georgia';
    src: url('assets/fonts/georgia.eot');
    src: local('☺'), url('assets/fonts/georgia.woff') format('woff'), url('assets/fonts/georgia.ttf') format('truetype'), url('assets/fonts/georgia.svg') format('svg');
    font-weight: normal;
    font-style: normal;
  }
  @font-face {
    font-family: 'times-new-roman';
    src: url('assets/fonts/times-new-roman.eot');
    src: local('☺'), url('assets/fonts/times-new-roman.woff') format('woff'), url('assets/fonts/times-new-roman.ttf') format('truetype'), url('assets/fonts/times-new-roman.svg') format('svg');
    font-weight: normal;
    font-style: normal;
  }

#app {
  font-family: 'times-new-roman', 'AriaMT', 'georgia', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
  @import "public/null_style";
</style>

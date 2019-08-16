<template>
  <div class="container">
    <div>
      <h1 class="title">
        CSTHINK
      </h1>
      <h2 class="subtitle">
        Comming Soon....
      </h2>
      <div class="links">
        <Button type="primary" target="_blank" to="https://tech.csthink.com/">
          技术团队
        </Button>
        <Button target="_blank" to="https://github.com/csthink">
          GitHub
        </Button>
      </div>
    </div>
  </div>
</template>

<script></script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 70px;
  letter-spacing: 1px;
  background-image: -webkit-linear-gradient(
    left,
    #22c1c3,
    #fdbb2d 25%,
    #22c1c3 50%,
    #fdbb2d 75%,
    #22c1c3
  );
  -webkit-text-fill-color: transparent;
  background-clip: text;
  background-size: 200% 100%;
  animation: myGradientChange 4s infinite linear;
  animation: myGradientChange 4s infinite linear;
}
@keyframes myGradientChange {
  0% {
    background-position: 0 0;
  }
  100% {
    background-position: -100% 0;
  }
}
.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}
.links {
  padding-top: 15px;
}
</style>

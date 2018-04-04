<template>
  <div class="row justify-center items-center">
    <div class="col-12 items-center">

      <div class="row justify-center">
        <h1>
          Hi!
          <img src="../assets/hand.png" alt="hand" class="hand">
        </h1>
      </div>
      <div class="row justify-center intro">
        <h3>
          My name is
        </h3>
      </div>
      <div class="row justify-center intro">
        <h2>
          Muhammad Shoman
        </h2>
      </div>

    </div>
  </div>

</template>

<script>
export default {
  name: 'Hello'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus">
@import '~variables'

.intro
  @-webkit-keyframes typing {
    from {
      width: 0;
    }
  }
  @-moz-keyframes typing {
    from {
      width: 0;
    }
  }
  @-webkit-keyframes blink-caret {
    from, to { border-color: white }
    10% { border-color: black }
  }
  h3
    width: 20%;
    white-space nowrap;
    border-right: 3px solid black;
    -webkit-animation: typing 1s steps(10), blink-caret 1s step-end 4s;
    -moz-animation: typing 1s steps(10), blink-caret 1s step-end 1s;
    overflow: hidden;
    -webkit-animation-delay 2s;
    -moz-animation-delay 2s;
    -webkit-animation-fill-mode:both;
    -moz-animation-fill-mode:both;

  h2
    width: 41%;
    white-space nowrap;
    border-right: 3px solid black;
    -webkit-animation: typing 1s steps(16), blink-caret 1s step-end infinite;
    -moz-animation: typing 1s steps(16), blink-caret 1s step-end infinite;
    overflow: hidden;
    -webkit-animation-delay 4s;
    -moz-animation-delay 4s;
    -webkit-animation-fill-mode:both;
    -moz-animation-fill-mode:both;

.hand
  -webkit-transform rotate(-40deg);
  -moz-transform rotate(-40deg);
  -o-transform rotate(-40deg);
  -ms-transform rotate(-40deg);
  transform rotate(-40deg);
  -webkit-animation wink .8s alternate infinite;
  -moz-animation wink .8s alternate infinite;
  -o-animation wink .8s alternate infinite;
  animation wink .8s alternate infinite;
  -webkit-transform-origin 50% 100%;
  -moz-transform-origin 50% 100%;
  -o-transform-origin 50% 100%;
  -ms-transform-origin 50% 100%;
  transform-origin 50% 100%;
  -webkit-animation-timing-function ease;
  animation-timing-function ease;
  @-webkit-keyframes wink {
    0% {
      -webkit-transform rotate(-40deg);
      -moz-transform rotate(-40deg);
      -o-transform rotate(-40deg);
      -ms-transform rotate(-40deg);
    }
    100% {
      -webkit-transform rotate(40deg);
      -moz-transform rotate(40deg);
      -o-transform rotate(40deg);
      -ms-transform rotate(40deg);
      transform rotate(40deg);
    }
}


</style>

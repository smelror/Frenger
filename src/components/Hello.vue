<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
var tracery = require('tracery-grammar')
var dict = tracery.createGrammar({
  'me': 'android automaton computer droid machine robot script'.split(' '),
  'you': ['friend', 'human', 'new friend', 'stranger', 'visitor'],
  'emotion': ['exicted', 'enthusiastic', 'empathic', 'friendly', 'happy'],
  'origin': 'Hello #you#, I\'m #emotion.a# #me#.'
})

export default {
  name: 'hello',
  data () {
    return {
      msg: dict.flatten('#origin#')
    }
  }
}
</script>

<style>
.hello h1 {
  color: #fff;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  font-size: 12vw;
  letter-spacing: -.4vw;
  line-height: 1.2em;
}
</style>

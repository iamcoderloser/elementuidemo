<template>
  <div class="hello">
    <h2>test</h2>
			<slot name='slotb'></slot>
			<slot></slot>
			<slot name='slotc'></slot>		
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>



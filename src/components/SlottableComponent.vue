<script>
  export default {
    render(h) {
      if (this.$slots.default.length !== 1) {
        throw new Error('Component requires one (1) root node for default slot. Can only deal with a single root DOM node.')
      }

      //Some logic that can only deal with one node here
      return h(this.$slots.default[0])
    }
  }
</script>

<style>

</style>

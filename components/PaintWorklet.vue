<script>
export default {
  functional: true,
  props: {
    src: {
      type: String,
      required: true
    }
  },
  render: function() {
    CSS.paintWorklet.addModule(this.src);
    return null;
  },
}
</script>
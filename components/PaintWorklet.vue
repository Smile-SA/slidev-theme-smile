<script>
export default function(props) {
  CSS.paintWorklet.addModule(props.src);
}
</script>
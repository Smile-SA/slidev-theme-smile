<script>
import { h } from 'vue';
export default function(props, { slots }) {
  if (slots.default) {
    return h('script', props, slots.default());
  }
}
</script>
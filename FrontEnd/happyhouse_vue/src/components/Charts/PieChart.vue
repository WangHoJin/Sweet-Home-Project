<script>
import { Pie } from "vue-chartjs";
export default {
  extends: Pie,
  // mixins: [reactiveProp],
  props: {
    chartdata: {
      type: Object,
      default: null,
    },
    options: {
      type: Object,
      default: null,
    },
  },
  mounted() {
    this.renderChart(this.chartdata, this.options);
  },
};
</script>

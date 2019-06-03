<template>
  <div class="card">
    <div class="card__stat">
      <div class="stat">
        <h5>{{label}}</h5>
        <h2>{{value}}</h2>
        <span>
            <span v-if="chart == 'completed'">
              <span class="green"><i class="fa fa-arrow-up"></i> {{rate}}</span>
            </span>
            <span v-else>
              <span class="red"><i class="fa fa-arrow-down"></i> {{rate}}</span>
            </span>
          </span>
      </div>
      <div>
        <span v-if="chart == 'number'">
          <img src="@/assets/Bar-Chart-2.svg" alt="chart"/>
        </span>
        <span v-else-if="chart == 'completed'">
          <img src="@/assets/Bar-Chart-1.svg" alt="chart"/>
        </span>
        <span v-else>
          <img src="@/assets/Bar-Chart.svg" alt="chart"/>
        </span>
      </div>
    </div>
  </div>
</template>
<script>

export default {
  data() {
    return {

    }
  },
  props: {
    label: String,
    value: Number,
    rate: Number,
    chart: String
  }
}
</script>
<style lang="scss" scoped>
  .card {
    width: 26%;
    background-color: #FFF;
    padding: 8px;
    margin-left: 35px;
    box-shadow: 2px 2px 2px 2px #EEE;
  }

  .card:nth-child(1) {
    margin-left: 0px !important;
  }

  .card h5 {
    margin: 0px;
    padding-top: 10px;
    color: #B3B3BD;
    font-weight: normal;
  }

  .card__stat {
    display: flex;
    padding-left: 10px;
    padding-right: 10px;
  }


  .card__stat > div:nth-child(2) {
    margin-left: auto;
    margin-top: 70px;
  }

  .card__stat h2 {
    margin-top: 40px;
    margin-bottom: 0px;
    padding: 0px;
    color: #666;
  }

  .card__stat > div:nth-child(1) > span {
    font-size: 12px;
  }

  .green {
    color: #3CC480;
  }

  .red {
      color: #FA696D;
  }
</style>

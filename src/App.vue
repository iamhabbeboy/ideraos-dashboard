<template>
  <div class="home">
    <div class="sidebar sidebar--mod">
      <Sidebar />
    </div>
    <div class="content">
      <Nav />
      <div class="container">
        <div class="order">
            <h3>Orders</h3>
            <div>
              <DatePicker />
            </div>
        </div>
        <div class="card__mod">
          <Card
            label="Number of Orders"
            value="246"
            rate="13.8%"
            chart="number"
            />
          <Card
            label="Completed Orders"
            value="246"
            rate="13.8%"
            chart="completed"
          />
          <Card
            label="Abadoned Orders"
            value="39"
            rate="13.8%"
            chart="abandoned"
          />
        </div>
        <div class="order-history--mod">
          <OrderHistory />
        </div>

      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Nav from '@/components/Nav.vue'
import Card from '@/components/Card.vue'
import Sidebar from '@/components/Sidebar.vue'
import DatePicker from '@/components/DatePicker.vue'
import OrderHistory from '@/components/OrderHistory.vue'

export default {
  name: 'home',
  components: {
    Nav,
    Card,
    Sidebar,
    DatePicker,
    OrderHistory
  }
}
</script>

<style lang="scss">
body {
  margin: 0px auto;
  font-family: 'Montserrat', sans-serif;
  font-family: 400;
  background: #FAFAFA;
}


.home {
  display: flex;
}

.sidebar--mod {
  width: 18% !important;
}

.container {
  width: 95%;
  margin-left: 20px;
}

.content {
  width: 82%;
  overflow:hidden;
}

.card__mod {
  display: flex;
  margin-top: 20px;
}

.order {
  display: flex;
  margin-top: 5px;
}

.order h3 {
  font-family: 'Lato', sans-serif;
  font-weight: 700;
  font-size: 1.3em;
  color: #1D91FF;
}

.order div {
  margin-left: auto;
  margin-top: 10px;
}

.order-history--mod {
  margin-top: 20px;
}


@media (max-width: 480px) {

  .home {
    display: block;
  }
    .content {
      width: 100% !important;
    }
    .container {
      width: 100% !important;
    }
}

</style>

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
            <input type="date" />
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
import OrderHistory from '@/components/OrderHistory.vue'

export default {
  name: 'home',
  components: {
    Nav,
    Card,
    Sidebar,
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
}

.order h3 {
  font-family: 'Lato', sans-serif;
  font-weight: 700;
  font-size: 1.3em;
  color: #1D91FF;
}

.order input {
  margin-left: auto;
}

.order-history--mod {
  margin-top: 20px;
}
</style>

<template>
  <div class="order-history">
    <h3>Order History </h3>
    <table class="order-history__table">
      <tr>
        <th>order id </th>
        <th>description </th>
        <th>payment method </th>
        <th> shipping method </th>
        <th>order amount </th>
        <th>date </th>
        <th>status </th>
      </tr>
      <tr>
        <td>0001</td>
        <td>Drizzle Grey Chambray </td>
        <td>Paystack</td>
        <td> MAX.NG </td>
        <td>&#8358; 30,000</td>
        <td>12/12/2001 </td>
        <td>
          <button class="danger">Abandoned</button>
        </td>
      </tr>
    </table>
  </div>
</template>

<style lang="scss" scoped>
.order-history {
  background: #FFF;
  padding: 10px;
}

.order-history__table {
  width: 95%;
  padding: 0px;
  margin: 0px auto;
  border-collapse: collapse;
  border-spacing: 0;

}

.order-history__table td {
  padding: 8px;
  text-align: center;
}

.order-history__table tr th {
  background: #ccc;
  padding: 10px;
}

.order-history__table tr td {
  border-bottom: 1px solid #ccc;

}

</style>

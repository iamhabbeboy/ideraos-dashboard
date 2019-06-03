<template>
  <div class="order-history">
    <h3>Order History </h3>
    <table class="order-history__table">
      <tr>
        <th>order id </th>
        <th class="width">description </th>
        <th>payment method </th>
        <th> shipping method </th>
        <th>order amount </th>
        <th>date </th>
        <th>status </th>
      </tr>
      <tr>
        <td>0001</td>
        <td><a href="#">Drizzle Grey Chambray Mix Women's Cabrillo Sneakers</a></td>
        <td>Paystack</td>
        <td> MAX.NG </td>
        <td>&#8358; 30,000</td>
        <td>12/12/2001 </td>
        <td>
          <button class="button danger">Abandoned</button>
        </td>
      </tr>
      <tr>
        <td>0002</td>
        <td><a href="#">Drizzle Grey Chambray </a></td>
        <td>Paystack</td>
        <td> MAX.NG </td>
        <td>&#8358; 30,000</td>
        <td>12/12/2001 </td>
        <td>
          <button class="button blue">In transit</button>
        </td>
      </tr>
      <tr>
        <td>0003</td>
        <td><a href="#">Drizzle Grey Chambray</a> </td>
        <td>Paystack</td>
        <td> MAX.NG </td>
        <td>&#8358; 30,000</td>
        <td>12/12/2001 </td>
        <td>
          <button class="button green">Completed</button>
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

.order-history h3 {
  margin-left: 8px;
  color: #666;
}

.order-history__table {
  width: 98%;
  padding: 0px;
  margin: 0px auto;
  border-collapse: collapse;
  border-spacing: 0;
  font-size: 13px;
}

.order-history__table td {
  padding: 8px;
  text-align: center;
  color: #666;
}

.order-history__table .width {
  width: 150px;
}

.order-history__table td a {
  color: #1D91FF;
  text-decoration: none;
}

.order-history__table tr th {
  background: #F5F6FA;
  padding: 15px;
  text-transform: uppercase;
  color: #999;
  font-size: 12px;
}

.order-history__table tr td {
  border-bottom: 1px solid #F7F7F8;
  padding-top: 15px;
  padding-bottom: 15px;
}

.button {
  padding: 5px 19px;
  width: 110px;
  background: #ccc;
  border-radius: 20px;
  border-color: transparent;
  color: #FFF;
}

.danger {
  background-color: #D80D04;
}

.blue {
  background-color: #1679EB;
}

.green {
  background-color: #3CC480;
}
</style>

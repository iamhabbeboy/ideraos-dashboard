<template>
  <div class="sidebar">
    <div class="logo-section">
      <img src="@/assets/Logo.svg" alt="Logo"/>
    </div>

    <ul class="links">
      <li><a href="#"><i class="fa fa-list"></i> Dashboard</a></li>
      <li><a href="#"><i class="fa fa-shopping-cart"></i> Products</a></li>
      <li><a href="#"><i class="fa fa-file"></i> Orders</a></li>
      <li><a href="#"><i class="fa fa-pie-chart"></i> Insight</a></li>
      <li><a href="#"><i class="fa fa-cog"></i> Settings</a></li>
    </ul>
  </div>
</template>

<style scoped>
.sidebar {
  background: #0F64C4;
  position: fixed;
  height: 100%;
  width: 18%;
  left: 0;
  top: 0;
}
.logo-section {
  background: #FFF;
  padding-bottom: 5px;
}

.links {
  margin: 60px auto;
}

.links li {
  list-style: none;
}

.links li a {
  text-decoration: none;
  color: #FFF;
  padding: 15px 10px;
  display: block;
}

@media (max-width: 480px) {
    .sidebar {
      display: none;
    }
}
</style>

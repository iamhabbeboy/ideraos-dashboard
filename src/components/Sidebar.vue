<template>
  <div class="sidebar">
    <div class="logo-section">
      <img src="@/assets/Logo.svg" alt="Logo"/>
    </div>
  </div>
</template>

<style lang="scss" scoped>
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
  padding-bottom: 3px;
}

@media (max-width: 400px) {
    .sidebar {
      display: none;
    }
}
</style>

<template>
  <section class="navbar">
    <div class="nav-block">
      <div>
        <div></div>
        <div class="search">
          <button>
            <i class="fa fa-search"></i>
          </button>
          <input type="text" placeholder="Search">
        </div>
        <div class="logo-section">
          <img src="@/assets/Logo.svg" alt="Logo"/>
        </div>
      </div>
      <div class="user-profile">
        <div>
          <a href="#">
            <i class="fa fa-bell"></i>
            <span class="notification">.</span>
          </a>
        </div>
        <div>Azeezat</div>
        <div>
          <a href="#">
            <i class="fa fa-chevron-down"></i>
            <i class="fa fa-user"></i>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss">
.navbar {
  width: 100%;
  padding: 20px;
  background: #FFF;
  box-shadow: 2px 2px 2px #ccc;
}

.nav-block {
  display: flex;
  width: 95%;
}

.logo-section {
  display: none;
}

.logo-section img {
  max-width: 100%;
  width: 80px;
}

.search button {
  background: transparent;
  border: transparent;
  color: #666;
  cursor:pointer;
  outline: none;
}

.search input[type=text] {
  background: transparent;
  border-color: transparent;
  font-size: 13px;
  outline: none;
}

.nav-block > div:nth-child(2) {
  margin-left: auto;
}

.user-profile {
  display: flex;
}

.user-profile a {
  color: #BCBCCB;
}

.user-profile > div {
  padding-left: 25px;
}

.user-profile > div:nth-child(1) {
  border-right: 1px solid #F3F3F7;
  padding-right: 20px;
}

.notification {
  font-size: 60px;
  color: orange;
  text-decoration: none;
  position: absolute;
  top: -35px;
  margin-top: 3px;
  margin-left: -6px;
}

.user-profile > div:nth-child(2) {
  font-weight: 600;
  font-size: 12px;
  color: #666;
}

.user-profile > div:nth-child(3) > a > i {
  padding-left: 10px;
}

@media (max-width: 400px) {
    .user-profile > div:nth-child(2) {
      display: none;
    }
    .user-profile > div:nth-child(3) {
      padding-left: 0px;
      padding-right: 10px;
    }
    .user-profile > div:nth-child(1) {
      padding-right: 0px;
    }

    .logo-section {
      display: block;
    }

    .search {
      display: none;
    }
}
</style>

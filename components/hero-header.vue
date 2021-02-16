<template>
  <header id="home">
    <div class="container">
      <nav class="navbar navbar-expand-lg navbar-dark">
        <img src="~static/images/logo.png" alt="logo" />
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "hero-header",
  data: () => {
    return {
      isActive: false
    };
  },
  methods: {
    scrollToElement() {
      // var element = document.getElementById("portfolioSection");
      // var top = element.offsetTop;
      // window.scrollTo(0, top);
    },
    myFilter: function() {
      this.isActive = !this.isActive;
      // some code to filter users
    }
  }
};
</script>

<style scoped lang="scss">
.header-liner {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
  color: #fff;
}

.menu {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-family: "lotasemibold";
  text-transform: uppercase;
  font-size: 18px;
}

header {
  width: 100%;
  background: none;

  li {
    text-align: right;
    font-family: "lotasemibold";
    font-size: 18px;
  }
}

@media (max-width: 768px) {
  .navbar .navbar-nav .nav-item .nav-link {
    padding-right: 0;
  }

  .navbar {
    padding: 8px 17px;
    margin: 0;
  }

  .navbar .navbar-toggler {
    background: none;
  }

  img {
    width: 100%;
  }
}

nav.navbar.navbar-expand-lg.navbar-dark {
  background: none;
  position: fixed;
  z-index: 50;
  left: 0;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: center;
}
</style>

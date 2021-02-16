<template>
  <!-- Main Parent Index Div -->
  <div class="main-parent">
    <header class="header-wrap">
      <!-- Import hero header -->
      <hero-header />
    </header>

    <div class="text">
      <p>
        We are currently upgrading our systems, please email
        <a href="mailto:service@craycraycrate.com">service@craycraycrate.com</a>
        for immediate assistance.
      </p>
    </div>

    <footer class="footer-wrap">
      <!-- Import fixed footer -->
      <fixed-footer />
    </footer>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Cray Cray Crate | A Gift Box Full of Greatness", // Grab title from API
      meta: [
        {
          hid: "description", //  Must use hid
          name: "description", // Type of meta property
          content: "A gift box for the ones you love, full of things they love."
        }
      ]
    };
  }
};
</script>

<style scoped>
.header-wrap {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  position: absolute;
  z-index: 40;
  width: 90%;
  left: 50%;
  margin-left: -45%;
  top: 30px;
}

.text {
  position: absolute;
  max-width: 510px;
  top: 50%;
  left: 50%;
  font-weight: 800;
  text-align: center;
  font-size: 20px;
  transform: translate(-50%, -50%);
  line-height: 30px;
}

@media (max-width: 768px) {
  .text {
    font-size: 14px;
    line-height: 20px;
  }
}

.footer-wrap {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  position: absolute;
  z-index: 40;
  width: 90%;
  left: 50%;
  margin-left: -45%;
  bottom: 30px;
}
</style>

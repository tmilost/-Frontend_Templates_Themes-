<template>
  <section class="main-view">
    <div class="container-scroller">
      <Header />
      <div class="container-fluid page-body-wrapper">
        <SettingsPannel></SettingsPannel>
        <!-- <Sidebar /> -->
        <div class="main-panel">
          <div class="content-wrapper">
            <router-view></router-view>
          </div>
          <!-- content wrapper ends -->
          <Footer />
        </div>
        <!-- main panel ends -->
      </div>
      <!-- page-body-wrapper ends -->
    </div>
  </section>
</template>

<script>
import Header from "./partials/Header";
// import Sidebar from "./partials/Sidebar";
import Footer from "./partials/Footer";
import SettingsPannel from "./partials/SettingsPannel";
export default {
  name: "layout",
  components: {
    Header,
    // Sidebar,
    Footer,
    SettingsPannel
  }
};
</script>

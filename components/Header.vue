<template>
  <div class="content_header_scroll">
<!--  <div class="content_header">-->
    <div class="container-fluid">
      <div class="row">
        <div class="col-sm-12 col-md-2 offset-md-1 col-lg-2 offset-lg-2">
          <a href="#"><img src="/img/logo_sogilis.svg"></a>
        </div>

        <nav class="col-md-7 offset-md-2 col-lg-6 offset-lg-1">
          <div class="dropdown">
            <button class="dropbtn">Services</button>
            <div class="dropdown-content">
              <nuxt-link to="/service-cloud-native-applications">
                {{ $t('services-cloud') }}
              </nuxt-link>
              <a href="#">{{ $t("service-iot") }}</a>
              <a href="#">{{ $t("service-critical") }}</a>
            </div>
          </div>
          <div class="dropdown">
            <button class="dropbtn">{{ $t("company") }}</button>
            <div class="dropdown-content">
              <a href="#" class="dropdown-content-company">{{ $t("company-vision") }}</a>
              <a href="#" class="dropdown-content-company">{{ $t("company-approach") }}</a>
            </div>
          </div>
          <a href="https://blog.sogilis.com" class="menu_link_1">Blog</a>
          <a href="#" class="menu_link_2">Contact</a>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
name: "Header"
}
</script>


<template>
  <div id="app">
    <div class="app-container app-theme-white body-tabs-shadow fixed-sidebar fixed-header">
      <div class="app-header header-shadow">
        <div class="app-header__logo ">
          <div class="logo-image">
            <img src="..\public\assets\images\logo-inverse.png" 
             width="100"
             height="50"
             alt=""
             class="d-inline-block align-top"
             >
          </div>
        </div>
        <div class="app-header__mobile-menu">
          
        </div>
        <div class="app-header__menu">
                <span>
                    <button type="button" class="btn-icon btn-icon-only btn btn-primary btn-sm mobile-toggle-header-nav">
                        <span class="btn-icon-wrapper">
                            <i class="fa fa-ellipsis-v fa-w-6"></i>
                        </span>
                    </button>
                </span>
        </div>
        <div class="app-header__content">
        <div class="app-header-left">
          
        </div>
        <div class="app-header-right">
          <div class="header-btn-lg pr-0">
            <div class="widget-content p-0">
              <div class="widget-content-wrapper">
                <div class="widget-content-left">
                  <div class="btn-group">
                    <a data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" class="p-0 btn">
                      <img width="42" class="rounded-circle" src="assets/images/avatars/1.jpg" alt="">
                      <i class="fa fa-angle-down ml-2 opacity-8"></i>
                    </a>
                    <div tabindex="-1" role="menu" aria-hidden="true" class="dropdown-menu dropdown-menu-right">
                      <button type="button" tabindex="0" class="dropdown-item">User Account</button>
                      <button type="button" tabindex="0" class="dropdown-item">Settings</button>
                    </div>
                  </div>
                </div>
                <div class="widget-content-left  ml-3 header-user-info">
                  <div class="widget-heading">
                    Admin
                  </div>
                  <div class="widget-subheading">
                    CS-1
                  </div>
                </div>
                <div class="widget-content-right header-user-info ml-2">
                  <i class="fa-solid pe-7s-user fa-2x"></i>
                </div>
                
              </div>
            </div>
          </div>        </div>
      </div>
      </div>
      <div class="ui-theme-settings">
      <button type="button" id="TooltipDemo" class="btn-open-options btn btn-warning">
        <i class="fa fa-cog fa-w-16 fa-spin fa-2x"></i>
      </button>
    </div>
      <div class="app-main">
      <div class="app-sidebar sidebar-shadow">
        <div class="app-header__logo">
          <div class="logo-src"></div>
          <div class="header__pane ml-auto">
            <div>
              <button type="button" class="hamburger close-sidebar-btn hamburger--elastic" data-class="closed-sidebar">
                                    <span class="hamburger-box">
                                        <span class="hamburger-inner"></span>
                                    </span>
              </button>
            </div>
          </div>
        </div>
        <div class="app-header__mobile-menu">
          <div>
            <button type="button" class="hamburger hamburger--elastic mobile-toggle-nav">
                                <span class="hamburger-box">
                                    <span class="hamburger-inner"></span>
                                </span>
            </button>
          </div>
        </div>
        <div class="app-header__menu">
                        <span>
                            <button type="button" class="btn-icon btn-icon-only btn btn-primary btn-sm mobile-toggle-header-nav">
                                <span class="btn-icon-wrapper">
                                    <i class="fa fa-ellipsis-v fa-w-6"></i>
                                </span>
                            </button>
                        </span>
        </div>    <div class="scrollbar-sidebar">
        <div class="app-sidebar__inner">
          <ul class="vertical-nav-menu">
            <li>
              <router-link to="/" active-class="mm-active" exact><i class="metismenu-icon pe-7s-home"></i> Beranda</router-link>
            </li>
            <li>
              <router-link to="/product" active-class="mm-active"><i class="metismenu-icon pe-7s-shopbag"></i> Produk</router-link>
            </li>
            <li>
              <router-link to="/about" active-class="mm-active"><i class="metismenu-icon pe-7s-info"></i> Tentang Kami</router-link>
            </li>
            <li>
              <router-link to="/contact" active-class="mm-active"><i class="metismenu-icon pe-7s-mail"></i> Hubungi Kami</router-link>
            </li>
            <li>
              <router-link to="/karyawan" active-class="mm-active"><i class="metismenu-icon pe-7s-users"></i> Karyawan</router-link>
            </li>
          </ul>
        </div>
      </div>
      </div>
        <div class="app-main__outer">
          <div class="app-main__inner">
            <router-view/>
          </div>
        </div>
    </div>
    </div>
  </div>
</template>

<style>
.logo {
    width: 100px;
}

.register input .login input {
    width: 300px;
    height: 40px;
    padding-left: 20px;
    display: block;
    margin-bottom: 30px;
    margin-right: auto;
    margin-left: auto;
    border: 1px solid skyblue;
}

.register button .login button {
    width: 320px;
    height: 40px;
    border: 1px solid skyblue;
    background: skyblue;
    color: #fff;
    cursor: pointer;
}
</style>


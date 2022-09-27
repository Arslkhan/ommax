<template>
    <div>
        <nav class="navbar">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">
                    <img src="../assets/Logo.png" alt="Logo" class="img-fluid" />
                </a>
                <button
                    class="navbar-toggler"
                    type="button"
                    data-bs-toggle="collapse"
                    data-bs-target="#collapsibleNavbar"
                    @click.prevent="menuDropdown()"
                >
                    <span id="navbar-toggler-icon" class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="collapsibleNavbar">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link line-bar" href="#"></a>
                        </li>
                        <li class="nav-item dropdown">
                            <a
                                class="nav-link dropdown-toggle"
                                href="#"
                                role="button"
                                data-bs-toggle="dropdown"
                                >Quick Facts</a
                            >
                            <ul class="dropdown-menu">
                                <li><a class="dropdown-item" href="#">Link</a></li>
                            </ul>
                        </li>
                        <li class="nav-item dropdown">
                            <a
                                class="nav-link dropdown-toggle"
                                href="#"
                                role="button"
                                data-bs-toggle="dropdown"
                                >Benefits</a
                            >
                            <ul class="dropdown-menu">
                                <li><a class="dropdown-item" href="#">Link</a></li>
                            </ul>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Contact</a>
                        </li>
                    </ul>
                </div>
                <button type="button" class="btn default-btn d-none d-md-block">
                    <div>Get In Touch</div>
                </button>
            </div>
        </nav>
        <div class="custom-menu" id="custom-menu">
            <ul>
                <li>
                    <a href="#">Quick Facts</a>
                </li>
                <li>
                    <a href="#">Benefits</a>
                </li>
                <li>
                    <a href="#">Contact</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: "Header",
  methods: {
    menuDropdown () {
      const menu = document.getElementById("custom-menu");
      menu.classList.toggle("show-menu");

      const menuBtn = document.getElementById("navbar-toggler-icon");
      menuBtn.classList.toggle("close");

      if (menuBtn.classList.contains("close")) {
        document.getElementsByTagName("body")[0].style.overflowY = "hidden";
      } else {
        document.getElementsByTagName("body")[0].style.overflowY = "unset";
      }
    }
  }
};
</script>

<style lang="scss" scoped>
.show-menu {
  display: block !important;
}
.overflowHide {
  overflow-y: hidden;
}
.custom-menu {
  display: none;
  @media (max-width: 660px) {
    width: 100%;
    height: 100vh;
    background: linear-gradient(rgba(0, 107, 110, 0.9), rgba(0, 107, 110, 0.9));
    position: absolute;
    left: 0;
    top: 7%;
    z-index: 1;
  }
  ul {
    background: #fff;
    padding: 2rem;
    margin-top: -1px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    list-style: none;
    text-align: center;

    li {
      border-bottom: 1px solid #cccccc;
      margin-bottom: 1.25rem;
      padding-bottom: 1.25rem;
      padding-top: 2rem;

      width: 100%;
      a {
        font-size: 1.25rem;
        color: #3d4d62;
        font-family: "IBMPlexBold", sans-serif;
        text-decoration: unset;
      }
    }

    li:last-child {
      border-bottom: unset;
    }
  }
}
.navbar {
  padding-left: 1.875rem;
  padding-right: 1.875rem;

  @media (max-width: 660px) {
    padding-left: 1rem;
    padding-right: 1rem;
    position: relative;
    z-index: 999;
  }
}
.nav-link {
  color: #3d4d62;
  font-family: "IBMPlexBold", sans-serif;
  font-size: 14px;

  &:hover {
    color: rgb(1, 164, 183);
  }
}
.navbar-toggler {
  border: unset;
}
.navbar-toggler:focus {
  box-shadow: unset;
}
.navbar-toggler-icon {
  width: 2rem;
  height: 2rem;
  background-image: url(../assets/menu.svg);
}
.navbar-toggler-icon.close {
  background-image: url(../assets/close.svg) !important;
}
.line-bar {
  background: #cccccc;
  height: 70px;
  width: 1px;
  padding: unset !important;
  @media only screen and (max-width: 660px) {
    display: none;
  }
}
.navbar-nav {
  align-items: center;

  @media (min-width: 800px) {
    gap: 50px;
  }
}
a.navbar-brand {
  margin-right: 3.7rem;
  img {
    @media (max-width: 660px) {
      width: 68%;
      border-right: 1px solid #cccccc;
      padding-right: 2rem;
    }
  }
}
</style>
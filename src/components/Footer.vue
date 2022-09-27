<template>
    <footer>
        <div class="container">
            <div class="footer-content">
                <ul>
                <li>
                    <a href="#">Imprint</a>
                </li>
                <li>
                    <a href="#">Data security</a>
                </li>
                <li>
                    <a href="#">Conditions</a>
                </li>
                <li>
                    <a href="#">Cookies</a>
                </li>
                <li>
                    <a href="#">Customs support</a>
                </li>
                </ul>
                <span> © 2021 Customs Support Group. All rights reserved. </span>
            </div>
        </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
footer {
  height: 120px;
  display: flex;
  width: 100%;
  align-items: center;
  .footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    @media only screen and (max-width: 775px) {
      flex-direction: column;
    }
    ul {
      padding: unset !important;
      margin: unset !important;
      list-style-type: none !important;
      li {
        display: inline-block;
        margin-right: 2rem;
        a {
          color: #3d4d62;
          font-family: "IBMPlexBold", sans-serif;
          font-size: 1rem;
          text-decoration: unset;
          &:hover {
            color: rgb(1, 164, 183);
          }
        }
      }
    }
    span {
      font-size: 0.75rem;
      @media only screen and (max-width: 775px) {
        margin-top: 1rem;
      }
    }
  }
}
</style>
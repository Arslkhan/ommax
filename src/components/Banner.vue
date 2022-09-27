<template>
    <section>
      <div class="mobile-overlay"></div>
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <h1 class="underline">
                        Headache on complex customs matters for your business?
                    </h1>
                    <p>
                        Customs Support is your neutral full-service customs broker for
                        complex customs matters with 20+ years of expertise in Europe and
                        over 400 customs specialists who are happy to take the load off your
                        mind!
                    </p>
                    <button class="btn default-btn d-none d-md-block">
                        Get your quote now
                    </button>
                </div>
                <div class="col-md-6 d-flex align-items-center">
                    <ul>
                        <li>Fast and accurate customs clearance delivery</li>
                        <li>EU-wide customs coverage</li>
                        <li>Online and real-time control of customs processes</li>
                    </ul>
                </div>
                <div class="col-md-12 d-flex d-md-none">
                    <button class="btn default-btn">Get your quote now</button>
                </div>
            </div>
        </div>
    </section>
  </template>

  <script>
  export default {
    name: "Banner",
  };
  </script>

  <style lang="scss" scoped>
  section {
    height: 690px;
    background: url("../assets/banner.png"),
      linear-gradient(rgba(0, 43, 44, 0.2), rgba(0, 43, 44, 0.2));
    background-blend-mode: overlay;
    position: relative;
    @media only screen and (max-width: 660px) {
      background-position: bottom;
    }
    .mobile-overlay {
      @media only screen and (max-width: 660px) {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgb(0, 107, 110);
        background: linear-gradient(
          180deg,
          rgba(0, 107, 110, 0) 27%,
          rgba(0, 107, 110, 1) 77%
        );
      }
    }
    .container {
      align-items: center;
      height: 100%;
      justify-content: center;
      display: flex;
      color: #fff;
      position: relative;
      @media only screen and (max-width: 660px) {
        padding: 0 2rem;
      }
      p {
        margin-bottom: 1.875rem;
      }
      ul {
        list-style: none;
        margin-left: 0;
        padding-left: 0;
  
        li {
          padding-left: 1em;
          text-indent: -1em;
          font-size: 1.25rem;
          font-family: "IBMPlexBold", sans-serif;
          margin-bottom: 1rem;
        }
  
        li:before {
          content: url("../assets/green-tick.svg");
          padding-right: 1rem;
        }
      }
      button {
        width: 12.875rem;
        @media only screen and (max-width: 660px) {
          width: 100%;
        }
      }
    }
  }
  </style>
  
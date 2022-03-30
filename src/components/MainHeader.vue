<template>
  <header fluid class="main-bg">
    <b-container class="header-bg d-flex flex-column justify-content-center">
      <h1 class="pb-5">
        Everyone gets phishing emails. Not everyone falls for them.
      </h1>
      <p>
        Find out the risk to your users from today’s biggest cyber threats in
        our eighth annual State of the Phish report.
      </p>
    </b-container>
  </header>
</template>


<script>
export default {
  name: "MainHeader",
};
</script>


<style scoped>
h1 {
  color: white;
  max-width: 500px;
}

p {
  color: white;
  font-size: 18px;
  max-width: 500px;
}
.main-bg {
  width: 100%;
  background-image: url(../assets/images/header.jpg);
  background-repeat: no-repeat;
  background-position: bottom;
}

.main-bg::after {
  content: "";
  position: absolute;
  top: 80px;
  left: 50%;
  width: 100%;
  transform: translate(-50%, 0);
  height: 550px;
  background: rgb(2, 92, 161);
  background: linear-gradient(
    137deg,
    rgba(2, 92, 161, 1) 23%,
    rgba(5, 108, 176, 1) 38%,
    rgba(12, 148, 212, 1) 90%
  );

  z-index: -1;
}

.header-bg {
  padding-top: 110px;
  min-height: 600px;
}
</style>

<template>
  <nav class="navheader">
    <h3 class="logotext">logo</h3>
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />
</template>

<style lang="scss">
$postcardBG: rgb(246, 246, 246);
$postcardShadowBG: #f3f3f3;

$postcardShadowBG2: #e0e0e0;

.navheader {
  -webkit-border-bottom-right-radius: 20px;
  -webkit-border-bottom-left-radius: 20px;
  -moz-border-radius-bottomright: 20px;
  -moz-border-radius-bottomleft: 20px;
  border-bottom-right-radius: 20px;
  border-bottom-left-radius: 20px;

  width: 70%;
  margin: 0 auto;
  padding: 10px;
  /* border: 1px solid black; */
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 1rem;
  background-color: $postcardBG;
  padding: 1rem;
  margin-bottom: 3rem;
  transition: 0.6s;
  -webkit-box-shadow: 0px 0px 17px 7px $postcardShadowBG;
  box-shadow: 0px 0px 17px 7px $postcardShadowBG;
  .logotext {
    flex: 1;
  }

  a {
    /* border: 1px solid pink; */
    text-decoration: none;
    padding: 7.7px;
    transition: 0.6s;
    -webkit-border-radius: 9px;
    -moz-border-radius: 9px;
    border-radius: 9px;
  }
  a:hover {
    background: orange;
  }
}

.navheader:hover {
  -webkit-box-shadow: 0px 0px 17px 7px $postcardShadowBG2;
  box-shadow: 0px 0px 17px 7px $postcardShadowBG2;
}

@media only screen and (max-width: 680px) {
  .navheader {
    width: 75%;
  }
}
</style>

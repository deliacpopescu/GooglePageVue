<template>
  <div id="footer">
    <p id="country">Romania</p>
    <div class="links">
      <div class="start">
        <a href="https://about.google/?utm_source=google-RO&utm_medium=referral&utm_campaign=hp-footer&fg=1">About</a>
        <a href="https://www.google.com/intl/ro_ro/ads/?subid=ww-ww-et-g-awa-a-g_hpafoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpafooter&fg=1"
          >Advertising</a>
        <a href="https://www.google.com/services/?subid=ww-ww-et-g-awa-a-g_hpbfoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpbfooter&fg=1"
          >Business</a>
        <a href="https://google.com/search/howsearchworks/?fg=1">How Search works</a>
      </div>
      <div class="end">
        <a href="https://policies.google.com/privacy?hl=ro&fg=1">Privacy</a>
        <a href="https://policies.google.com/terms?hl=ro&fg=1">Terms</a>
        <a href="www.google.com">Settings</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  main: "Footer",
};
</script>

<style scoped>
#footer {
  background-color: #f2f2f2;
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 80px;
  font-size:14px;
}
#country {
  /* line-height: 30px; */
  margin-left: 10px;
  text-align: left;
  border-bottom: 1px solid rgb(199, 199, 199);
}
.links{
    display:flex;  
    flex-wrap: wrap;
    /* justify-content: space-evenly; */
    justify-content: space-between;

}
p{
    color: #70757a;
}
a {
  color: #70757a;
  padding:15px;
  text-decoration: none;
  
}
a:hover {
  color: #70757a;
  text-decoration: underline;
}
</style>

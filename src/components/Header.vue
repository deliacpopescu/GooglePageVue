<template>
  <div class="header">
    <div class="header-links">
      <div class="links">
        <a href="https://www.google.com/">Gmail</a>
      </div>
      <div class="links">
        <a href="https://www.google.ro/imghp?hl=en&ogbl">Images</a>
      </div>
      <div class="links">
        <button id="menu-btn">
          <img alt="menu button" src="./../assets/dots-menu.svg" />
        </button>
      </div>

      <div class="links">
        <button id="email-btn">D</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  main: "Header",
};
</script>

<style scoped>
.header {
  height: 60px;
}
.header-links {
  display: inline-flex;
  float: right;
  align-items: center;
}
.links {
  padding-right: 20px;
}
a {
  color: rgba(0, 0, 0, 0.87);
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
#menu-btn img {
  height: 1rem;
}
#menu-btn {
  border: none;
  background-color: transparent;
}
#menu-btn:hover {
  cursor: pointer;
  border: none;
  box-shadow: 0px 1px 1px rgba(194, 192, 192, 0.15);
}

#email-btn {
  height: 32px;
  width: 32px;
  background-color: darkblue;
  border: none;
  border-radius: 50%;
  color: white;
}
</style>

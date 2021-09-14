<template>
  <div id="main">
    <div id="container">
      <div>
        <img id="logo" alt="google logo" src="./../assets/Google_logo.png" />
      </div>
      <div>
        <div>
          <img id="lupe" src="./../assets/lupe.png" alt="lupe" />
          <input id="search-bar" type="text" />
          <img id="mic" src="./../assets/Google_mic.svg.png" alt="microphone" />
        </div>
        <div class="btns">
          <button type="button" class="btn">Google Search</button>
          <button type="button" class="btn">I'm Feeling Lucky</button>
        </div>
        <div id="language">
          <p>Google offered in:</p>
          <a href="https://www.google.com/setprefs?sig=0_n02S24IAL8XhmM1Ccg-7v2JhgVc%3D&hl=ro&source=homepage&sa=X&ved=0ahUKEwiLxqmH5NvyAhUC7XMBHVKgBWgQ2ZgBCA8"
            >Romana</a
          >
          <a href="https://www.google.com/setprefs?sig=0_n02S24IAL8XhmM1Ccg-7v2JhgVc%3D&hl=hu&source=homepage&sa=X&ved=0ahUKEwiLxqmH5NvyAhUC7XMBHVKgBWgQ2ZgBCBA"
            >Magyar</a
          >
          <a href="https://www.google.com/setprefs?sig=0_n02S24IAL8XhmM1Ccg-7v2JhgVc%3D&hl=de&source=homepage&sa=X&ved=0ahUKEwiLxqmH5NvyAhUC7XMBHVKgBWgQ2ZgBCBE"
            >Deutsch</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  main: "Main",
};
</script>

<style scoped>
#main {
  height: calc(100% - 60px);
  margin-top: 10rem;
}
#logo {
  max-height: 92px;
}
#search-bar {
  margin-top: 1rem;
  height: 44px;
  width: 40%;
  border: 1px solid #dfe1e5;
  border-radius: 24px;
  box-shadow: none;
}
.btns {
  margin-top: 2rem;
}
.btn {
  height: 36px;
  width:150px;
  margin: 0.5rem;
  border: none;
  border-radius: 4px;
  background-color: #f8f9fa;
}
.btn:hover{
    border:1 px solid black;
    box-shadow: 0 1px 3px rgb(32 33 36 / 28%);
    }
#lupe {
  width: 30px;
  position: absolute;
  margin-top: 32px;
  margin-left: 10px;
  color: #9aa0a6;
}
#keyboard {
  width: 30px;
  position: absolute;
  margin-left: -80px;
  margin-top: 7px;
  color: #9aa0a6;
}
#mic {
  width: 15px;
  position: absolute;
  margin-left: -40px;
  margin-top: 30px;
}

#search-bar:hover {
  box-shadow: 0 1px 6px rgb(32 33 36 / 28%);
}
#language {
  display:inline-flex;
  margin-top: 10px;
  margin-left: 10px;
}
#language p{
    margin:0;
    padding-right: 10px;
}
#language a {
  color: #1a0dab;
  padding-right: 10px;
  text-decoration: none;
}
#language a:hover {
  text-decoration: underline;
}
</style>

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
        <button id="menu-btn" v-on:click="isHidden=!isHidden">
          <img alt="menu button" src="./../assets/dots-menu.svg" />
        </button>
         <div v-if="!isHidden" class="google-apps">
                    <!-- <div class="d-flex justify-content-around mt-3 mb-3"> -->
                        <img src="./../assets/calendar.png" alt="calendar"/>
                        <img src="./../assets/drive.png" alt="drive"/>
                        <img src="./../assets/gmail.png" alt="gmail"/>
                    <!-- </div>   
                    <div class="d-flex justify-content-around mt-3">      -->
                        <img src="./../assets/gmap.png" alt="gmap"/>
                        <img src="./../assets/photos.png" alt="photos"/>
                        <img src="./../assets/youtube.png" alt="youtube"/>
                    <!-- </div> -->
                </div>
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
  data(){
      return{
          isHidden:true
      }
      }
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
  width: 32px;
  height: 32px;
}
#menu-btn:hover {
  cursor: pointer;
  background-color: #dadce0;
  border-radius: 50%;
}
#email-btn {
  height: 32px;
  width: 32px;
  background-color: darkblue;
  border: none;
  border-radius: 50%;
  color: white;
}

.google-apps{
    background: white;
    -webkit-border-radius: 4px;
    border-radius: 4px;
    border:1px solid grey;
    box-shadow: 2px 2px #888888;
    top:60px;
    margin-right: 20px;
    padding: 4px 8px;
    position: absolute;
    height:200px;
    width: 200px;
    right:0;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.google-apps img{
    width:50px;
    height:50px;
    margin:7px;
}
</style>

<template>
  <header class="header">
    <nav class="nav">
      <div class="nav__content container">
        <div class="logo">
          <a href="#"><img src="../assets/images/ui.svg" alt="logo"></a>
          <h3 class="logo-name">Notitanic</h3>
        </div>
        <div class="nav">
          <ul class="nav-list">
            <li class="li"><a href="#" class="nav-list-item">Home</a></li>
            <li class="li"><a href="#about" class="nav-list-item">About me</a></li>
            <li class="li"><a href="#portfolio" class="nav-list-item">Portfolio</a></li>
            <li class="li"><a href="#contact" class="nav-list-item">Contact</a></li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
  export default{}


</script>

<style>
@media (max-width:1199.99px) {
  .nav-list{
    gap: 50px !important;
  }
}
@media (max-width:991.99px){
  .nav-list{
    position: absolute;
    top: 0;
    right: 0;
    margin-right: 0 !important;
    gap: 30px !important;
    flex-direction: column;
  }
}
  .li{
    cursor: pointer;
    z-index: 3;
}
.header{
  background: var(--bg1, linear-gradient(102deg, #2C2C2C 1.56%, #1C1C1C 95.55%));
  padding: 20px 0;
  position: relative;
}
.logo{
  display: flex;
  flex-direction: row;
  gap: 10px;
  align-items: center;
}
.logo-name{
  color: white;
  font-family: NicoMoji;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
.nav-list-item{
  color: var(--text, #E4E4E4);
  font-family: Arodora-Pro;
  font-size: 18px;
  font-style: normal;
  font-weight: 300;
  cursor: pointer;
}
.nav-list-item :hover{
  cursor: pointer;
}
.nav__content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.nav-list{
  display: flex;
  gap: 145px;
  margin-right: 100px;
}
</style>
<template>
  <header>
      <div class="container">
            <nav class="row">
                <div class=" col-md-6 col-6 logo_tag">
                    <img src="../assets/pngwing.com-removebg-preview.png" alt=""><span><b>BRIGHT</b></span>
                </div>
                <div class=" col-md-6 col-6 sidebar_icon">
                    <div class="sidebar">
                        <button class="btn" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasRight"
                            aria-controls="offcanvasRight"><i class="bi bi-justify-right"></i></button>

                        <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasRight"
                            aria-labelledby="offcanvasRightLabel">
                            <div class="offcanvas-header">
                                <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas"
                                    aria-label="Close"></button>
                            </div>
                            <div class="offcanvas-body">
                                <div class="sidebar-route">
                                    <p><router-link :to="{ name: 'Home' }">Home</router-link></p><br>
                                    <p><router-link :to="{ name: 'About' }">About</router-link></p><br>
                                    <p><router-link :to="{ name: 'Portfolio' }">Portfolio</router-link></p><br>
                                    <p><router-link :to="{ name: 'Contact' }">Contact</router-link></p><br>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </nav>
        </div>
  </header>
</template>

<script>
export default {

}
</script>

<style>
body{
    background-color: #212121;
}
.logo_tag img {
    width: 3rem;
    height: 3rem;
}
.logo_tag span {
    font-family: cursive;
    color: white;
}
.sidebar_icon{
    text-align: right;
}
.btn:focus, .btn:active:focus, .btn.active:focus{
    outline:none;
    box-shadow:none;
}
.btn-close:focus, .btn-close:active:focus, .btn-close.active:focus{
    outline:none;
    box-shadow:none;
}
.sidebar_icon button i{
    color: #7a93d8;
    height: 4rem;
    width: 4rem;
}
.offcanvas{
    width: 14rem;
    background-color: #212121;
}
.sidebar-route{ 
    text-align: center;
}
.sidebar-route p{ 
    display: flex;
    justify-content: center;
}
.sidebar-route a{ 
    color: white;
    text-decoration: none;
    font-weight: bold;
    width: 7rem;
    background-color: #7a93d8;
    box-shadow: 0 1px 2px grey;
    padding: 0.4rem;
    border-radius: 0.4rem;
}
.sidebar-route a:hover{ 
    background-color: #232e4e;
}
.sidebar-route a.router-link-exact-active{ 
    background-color: #232e4e;
}
</style>
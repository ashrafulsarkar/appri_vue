<script setup>
    // sticky
    $(window).on('scroll', function () {
        var scroll = $(window).scrollTop();
        if (scroll < 2) {
            $("#header-sticky").removeClass("sticky");
        } else {
            $("#header-sticky").addClass("sticky");
        }
    });
</script>
<template>
    <header>
        <div id="header-sticky" class="header-area transparent-header pt-40 pb-40">
            <div class="container">
                <div class="row align-items-center">
                    <div class="col-xl-2 col-lg-2">
                        <div class="logo">
                            <a href="/"><img src="/img/logo/logo.png" alt=""></a>
                        </div>
                    </div>
                    <div class="col-xl-8 col-lg-8">
                        <div class="main-menu">
                            <nav  id="mobile-menu" class="navbar navbar-expand-lg navbar-dark">
                                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarToggler" aria-controls="navbarToggler" aria-expanded="false" aria-label="Toggle navigation">
                                    <span class="navbar-toggler-icon"></span>
                                </button>
                                <div class="collapse navbar-collapse" id="navbarToggler">
                                    <ul class="navbar-nav">
                                        <li><a href="#home">Home</a></li>
                                        <li><a href="#features">Features</a></li>
                                        <li><a href="#pricing">Pricing</a></li>
                                        <li><a href="#screenshot">Screenshot</a></li>
                                        <li><a href="#faq">Faq</a></li>
                                        <li><a href="#news">News</a></li>
                                    </ul>
                                </div>
                            </nav>
                        </div>
                    </div>
                    <div class="col-lg-2 d-none d-lg-block">
                        <div class="header-btn">
                            <a href="#" class="btn">Sign In</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>        
    </header>
</template>
<style scoped>
.main-menu #navbarToggler {
    justify-content: center;
}
@media screen and (max-width:991px) {
    .main-menu nav {
        justify-content: flex-end;
        padding: 0;
    }
    .main-menu {
        margin-top: -47px;
    }
    .main-menu nav ul {
        background: #fff;
        margin-top: 20px;
    }
    .main-menu nav ul li a {
        color: #000;
    }
}
</style>
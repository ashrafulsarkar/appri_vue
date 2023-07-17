<script setup>
    // ===== Scroll to Top ==== 
    $(window).scroll(function () {
        if ($(this).scrollTop() >= 5000) {
            $('#return-to-top').fadeIn(300);
        } else {
            $('#return-to-top').fadeOut(300);
        }
    });
    function returnTop() {
        $('body,html').animate({
            scrollTop: 0
        }, 500);
    };
</script>
<template>
    <footer class="footer-area">
        <div class="container">
            <div class="row">
                <div class="col-xl-12">
                    <div class="copy-right text-center pt-40 pb-40">
                        <p>2023 Copyright Appri App Landing Designed by Love. All Rights Reserved</p>
                    </div>
                </div>
            </div>
        </div>
        <div><a href="javascript:" @click="returnTop" id="return-to-top"><i class="fas fa-chevron-up"></i></a></div>
    </footer>
</template>
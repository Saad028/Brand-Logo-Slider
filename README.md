# Brand-Logo-Slider
we had to add below link under the {{ 'theme.css' | asset_url | stylesheet_tag }} link.
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/assets/owl.theme.default.css">
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/assets/owl.carousel.min.css">


we had to add below script under the theme.js file inside the body
<script> src="{{ 'empire.js' | asset_url }}" </script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/OwlCarousel2/2.3.4/owl.carousel.min.js"></script>
<script>

  $('.owl-carousel').owlCarousel({
     items : 5,
    loop:true,
    autoplay: true,
    stagePadding: 50,
    margin:40,
    nav:true,
    dots: false,
    navText : ["<i class='fa fa-chevron-left'></i>","<i class='fa fa-chevron-right'></i>"],
    responsiveClass:true,
    responsive:{
        0:{
            items:1,
            nav:false,
            dots: false
        },
        600:{
            items:3,
            nav:true
        },
        1000:{
            items:5,
            nav:true,
            loop:true
        }
    }
})
  
  
</script>

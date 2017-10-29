# lightbox_js
The well known but original old LightBox with some enhancements.

The oldy but well known javascript LightBox v 1 with no dependencies that helped us in the '2000s to create simple but effective photo galleries.
This is a version adapted and corrected for a better cross-browser support, responsive and with capacities for multilanguage. Minified within Babel JS to follow the new generation of coding. Only 8 kbytes (js & CSS files combined) before Gzip compression; IE6 minimum. Because speed matters.

# Additional CSS rules if needed

    <!--[if lte IE 6]>
    <style>
    /*! IE5-6 just because LightBox 1 seems to work fine with it :D */
    body {overflow-x: hidden}
    /* The wrapper of your gallery */
    .gallery {width: 97.5%!important}
    /* Needed: corrects some ugly things */
    #lightbox {left:0!important}
    .thumb-image {width: auto!important}
    </style>
    <![endif]-->

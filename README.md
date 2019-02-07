# lightbox_js

The well known but original old LightBox with some enhancements.

The oldy but well known javascript LightBox v 1 with no dependencies that helped us in the '2000s to create simple but effective photo galleries.
This is a version adapted and corrected for a better cross-browser support, responsive and with capacities for multilanguage. Minified within Babel JS to follow the new generation of coding. Only 8 kbytes (js & CSS files combined) before Gzip compression; IE6 minimum. With no dependencies because speed matters.

## Configuration

Add the styles and the script files localy into your pages or:

`<link rel="stylesheet" href="//cdn.jsdelivr.net/gh/cara-tm/lightbox_js/css/lightbox.min.css" />`

`<script src="//cdn.jsdelivr.net/gh/cara-tm/lightbox_js/lightbox_js.min.js"></script>`

You have access to some variables in order to configure the script depending of your needs and/or pretty suitable for translations:

* `close_string` The string displayed on the right bottom of your images.
* `close_tooltip` The tooltip title for the Close button.
* `loadingImage` The path to your custom loading image.

So place this into your pages:

    <script>
    var close_string = 'press <a href="#" onclick="hideLightbox(); return false;"><kbd>x</kbd></a> to close',
    close_tooltip = 'Click to close',
    loadingImage = '/img/white-loader.gif',closeButton='/img/close.gif';
    </script>
    
## Putting it all files together

All files required are available within two CDN services. Here is the samples of integration.

### jsDelivr

    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/cara-tm/lightbox_js@1.0/css/lightbox.min.css" />

    <script src="https://cdn.jsdelivr.net/gh/cara-tm/lightbox_js@1.0/lightbox_js.min.js"></script>
    <script>
    var close_string = 'press <a href="#" onclick="hideLightbox(); return false;"><kbd>x</kbd></a> to close',
    close_tooltip = 'Click to close',
    loadingImage = '/img/white-loader.gif',closeButton='/img/close.gif';
    </script>

### RawGit

    <link rel="stylesheet" href="https://cdn.rawgit.com/cara-tm/lightbox_js/0a8a14f3/css/lightbox.min.css">
    
    <script src="https://cdn.rawgit.com/cara-tm/lightbox_js/0a8a14f3/lightbox_js.min.js"></script>
    <script>
    var close_string = 'press <a href="#" onclick="hideLightbox(); return false;"><kbd>x</kbd></a> to close',
    close_tooltip = 'Click to close',
    loadingImage = '/img/white-loader.gif',closeButton='/img/close.gif';
    </script>

## Additional CSS rules if needed

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

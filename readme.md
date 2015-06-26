# Kirby Gallery

A gallery plugin for [Kirby 2](http://getkirby.com) that uses [Zurb Foundation][1].

## Instillation
1. Place gallery.php in your site/plugins directory.
2. Place site/blueprints/gallery.php in your site/blueprints directory.

### Not Using Foundation?
If you are not already using Foundation, there are a couple additional steps:

1. Place foundation.css in your asstes/css directory.
2. Place the contents of assets/js in your assets/js directory.
3. In your snippets/header.php include:
```html
<?php echo css("assets/css/foundation.css") ?>
<?php echo js("assets/js/vendor/modernizr.js") ?>`
```
4. In your snippets/footer.php include:
```html
  <?php js("assets/js/vendor/jquery.js") ?>
  <?php js("assets/js/foundation.min.js") ?>
  <script>
    $(document).foundation();
  </script>
```

## Usage

Show a gallery on a page using `<?php echo getGallery($page, $galleryUri) ?>`


[1](http://foundation.zurb.com/)

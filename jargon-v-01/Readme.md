# WordPres

## Setting Up The Index.template

1. create index.php
1. add basic web page template markup.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Jargon</title>
</head>
<body>
       <nav></nav>
       <header></header>
       <main></main>
       <footer></footer>
</body>
</html>

```
1. Copy everthing up to the end of the header tag and add it to your header.php file. Right before the end of the head element add the WP code snippet wp_head();. Make sure you spell it correctly and formatted correctly.
```php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Jargon</title>
    <?php wp_head();  ?>
</head>
<body>
       <nav></nav>
       <header></header>

```
1. Now copy the footer element down to the closing html element
```php
       <footer></footer>
       <?php wp_footer(); ?>
</body>
</html>

```
1. Now in your index.php document call the page header and footer in to your document.

```php
      <?php get_header(); ?>
      <main>Index Template</main>
       <?php get_footer(); ?>
</body>
</html>
```


1. create style.css
1. copy and paste the style.css meta data from the [WordPresss Developers Handbook](https://developer.wordpress.org/themes/basics/main-stylesheet-style-css/) and add it to your css file.


```css

/*
Theme Name: Your Theme name
Theme URI: url to the theme
Author: developer name
Author URI: developer site address
Description: This all shows up in the theme panel in the themes section
Version: 1.0 (version number)
License: GNU General Public License v2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Text Domain: theme name one word
Tags: Used to find you theme when a users searches in the themes panel.
*/
```
### Get Widget Data

Get raw data from standard Wordpress widget instances.

#### Usage

This will return an array of data from the widget with the name 'Homepage hero banner'. In this instance it's getting the urls of images added to the widget and wrapping them in an image tag.

```php
if ( is_active_sidebar( 'homepage_hero_banner' ) ){
    $widgetData = get_widget_data('Homepage hero banner');
    foreach($widgetData as $data){
        $imgUrl = $data->url;
        echo '<img src="'.$imgUrl.'"/>';
    }
}
```

```

   |\          .(' *) ' .
   | \        ' .*) PHP .'*
   |(*\      .*(// .*) .
   |___\       // (. '*
   ((("'\     // '  * .
   ((c'7')   /\)
   ((((^))  /  \
 .-')))(((-'   /
    (((()) __/'
     )))( |
      (()
       ))

```

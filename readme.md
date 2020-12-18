## Get Widget Data

Get raw data from standard Wordpress widget instances.

#### Usage

```php
if ( is_active_sidebar( 'homepage_hero_banner' ) ){
    $widgetData = get_widget_data('Homepage hero banner');
    foreach($widgetData as $data){
        $imgUrl = $data->url;
        echo '<div class="banner" style="background-image: url('.$imgUrl.');"></div>';
    }
}
```

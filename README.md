# Yii2-swiper  fixed version romka-chev/yii2-swiper
## Installation
 
You can get this extension through [Composer](https://getcomposer.org/download/).
 
Either run in terminal
 
```Shell
$ php composer.phar require "sinelnikof/yii2-swiper" "*"
```
 
or add
 
```JSON
"sinelnikof/yii2-swiper" : "*"
```
 
to the *require* section of your application's ```composer.json``` file.
    
###Usage

```PHP
 
<?php
/**
 * @var \yii\web\View $this
 */
use sinelnikof\yii2\swiper\Swiper;

echo Swiper::widget( [
  'items'         => [
    [ 'background' => 'http://lorempixel.com/600/600/nature/1' ],
    [ 'background' => 'http://lorempixel.com/600/600/nature/2' ],
    [ 'background' => 'http://lorempixel.com/600/600/nature/3' ],
    [ 'background' => 'http://lorempixel.com/600/600/nature/4' ],
    [ 'background' => 'http://lorempixel.com/600/600/nature/5' ]
  ],
  'behaviours'    => [
    'pagination'
  ],
  'pluginOptions' => [
    'grabCursor'     => true,
    'centeredSlides' => true,
    'slidesPerView'  => 'auto',
    'effect'         => 'coverflow',
    'coverflow'      => [
        'rotate'       => 50,
        'stretch'      => 0,
        'depth'        => 100,
        'modifier'     => 1,
        'slideShadows' => true
    ]
  ]
] );
 
```

## Issues
 

[![Build Status](https://travis-ci.com/seatplus/eseye.svg?branch=master)](https://travis-ci.com/seatplus/eseye)
Code Coverage
Test Coverage
[![Latest Stable Version](https://poser.pugx.org/seatplus/eseye/v/stable)](https://packagist.org/packages/seatplus/eseye)
[![Total Downloads](https://poser.pugx.org/seatplus/eseye/downloads)](https://packagist.org/packages/seatplus/eseye)
[![License](https://poser.pugx.org/seatplus/eseye/license)](https://packagist.org/packages/seatplus/eseye)
[![StyleCI](https://github.styleci.io/repos/216053626/shield?branch=master)](https://github.styleci.io/repos/216053626)


# eseye
🛰️🛰️🛰️ A fork of eveseat/eseye: A Standalone PHP ESI (EVE Swagger Interface) Client Library. Supports Monolog ^2.0 and php redis

## example usage
Its supposed to be simple!

```php
// initialization stuff
$esi = new Eseye();

// Optionally, set the ESI endpoint version to use.
// If you dont set this, Eseye will use /latest
$esi->setVersion('v4');

// make a call
$character_info = $esi->invoke('get', '/characters/{character_id}/', [
    'character_id' => 1477919642,
]);

// get data!
echo $character_info->name;
```

For a more complete usage example, please refer to [example.php](example.php)

## documentation
For up to date documentation, more examples and other goodies, please check out the [project wiki](https://github.com/eveseat/eseye/wiki)!

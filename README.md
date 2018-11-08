# Google Street View API

[![Latest Version](https://img.shields.io/github/release/defro/google-streetview.svg?style=flat-square)](https://github.com/defro/google-streetview/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/defro/google-streetview/master.svg?style=flat-square)](https://travis-ci.org/defro/google-streetview)
[![SensioLabsInsight](https://img.shields.io/sensiolabs/i/c0e7c71d-351a-4996-9d74-24abfa074410.svg?style=flat-square)](https://insight.sensiolabs.com/projects/c0e7c71d-351a-4996-9d74-24abfa074410)
[![StyleCI](https://styleci.io/repos/156726302/shield)](https://styleci.io/repos/156726302)
[![Total Downloads](https://img.shields.io/packagist/dt/defro/google-streetview.svg?style=flat-square)](https://packagist.org/packages/defro/google-streetview)

This package can get street view image from any address to GPS coordinates, location or panorama ID using [Google's street view service](https://developers.google.com/maps/documentation/streetview/intro). Here's a quick example:

```php
$client = new \GuzzleHttp\Client();
$streetView = new \Defro\Google\StreetView\StreetView($client);
$imgUrl = $streetView
    ->setApiKey('YOUR_GOOGLE_API_KEY')
    ->getImageUrlByAddress('Eiffel tower, Paris');

echo '<img src="' . $imgUrl . '" />';
```

## Documentation

Read to install, use this package, customize image to display on [documentation page](https://defro.github.io/google-streetview/).


## License

The MIT License (MIT). Please see [license File](LICENSE.md) for more information.

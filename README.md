# Adobe Sign Provider for OAuth 2.0 Client

https://acrobat.adobe.com/us/en/sign.html

This package provides Adobe Sign OAuth 2.0 support for The PHP League's [OAuth 2.0 Client](https://github.com/thephpleague/oauth2-client).
Forked from the great work of Kevin Em for V5 Adobe API https://github.com/kevinem/oauth2-adobe-sgin

[![Latest Stable Version](https://poser.pugx.org/eazieer/oauth2-adobe-sign-v6/v/stable?format=flat-square)](https://packagist.org/packages/eazieer/oauth2-adobe-sign-v6)
[![License](https://poser.pugx.org/eazieer/oauth2-adobe-sign-v6/license?format=flat-square)](https://packagist.org/packages/eazieer/oauth2-adobe-sign-v6)
[![Build Status](https://travis-ci.org/eazieer/oauth2-adobe-sign-v6.svg?branch=master)](https://travis-ci.org/eazieer/oauth2-adobe-sign-v6)

## Installation

To install, use composer:

```
composer require eazieer/oauth2-adobe-sign-v6
```

## Usage

Use [The League's OAuth2 Client](https://github.com/thephpleague/oauth2-client) with `\Eazieer\OAuth2\Client\AdobeSign` as the provider.

### Authorization Code Flow

```php
$provider = new Eazieer\OAuth2\Client\AdobeSign([
    'clientId'          => 'your_client_id',
    'clientSecret'      => 'your_client_secret',
    'redirectUri'       => 'your_callback',
    'dataCenter'        => 'secure.na1',
    'scope'             => [
          'scope1:type',
          'scope2:type'
    ]
]);
```

## License 

The MIT License (MIT)
Copyright (c) 2016 Kevin Em

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
documentation files (the "Software"), to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of
the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
IN THE SOFTWARE.

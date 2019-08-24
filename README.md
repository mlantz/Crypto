# Crypto

**Crypto** - Powerful and elegant cryptography tools for Laravel and Lumen

[![Build Status](https://travis-ci.org/GrafiteInc/Crypto.svg?branch=master)](https://travis-ci.org/GrafiteInc/Crypto)
[![Maintainability](https://api.codeclimate.com/v1/badges/7577ab93d33bf9b69605/maintainability)](https://codeclimate.com/github/GrafiteInc/Crypto/maintainability)
[![Packagist](https://img.shields.io/packagist/dt/grafite/crypto.svg?maxAge=2592000)](https://packagist.org/packages/grafite/crypto)
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://packagist.org/packages/grafite/crypto)

The Cryptograpy toolset Crypto provides a collection of methods for handy, encryption, decryption, uuid generating, app key generating and more.

##### Author(s):
* [Matt Lantz](https://github.com/mlantz) ([@mattylantz](http://twitter.com/mattylantz), mattlantz at gmail dot com)

## Requirements

1. PHP 5.6+
2. OpenSSL
3. Laravel 5.3+ or Lumen

* For Lumen you must enable Facades: `$app->withFacades()`

----

### Installation

Start a new Laravel project:
```php
composer create-project laravel/laravel your-project-name
```

Then run the following to add Crypto
```php
composer require "grafite/crypto"
```

## Documentation

##### encrypt()

```
Crypto::encrypt('testing');

// helper
crypto_encrypt();
```

##### decrypt()

```
Crypto::decrypt('encrypted-text');

// helper
crypto_decrypt();
```

##### uuid()

```
Crypto::uuid();

// helper
crypto_uuid();
```

##### shareable()

The shareable as mentioned uses a common encryption key so that the encrypted values can be shared.

```
Crypto::shareable()->encrypt('testing');
Crypto::shareable()->decrypt('encrypted-text');
```


## License
Crypto is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)

### Bug Reporting and Feature Requests
Please add as many details as possible regarding submission of issues and feature requests

### Disclaimer
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

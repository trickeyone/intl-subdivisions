IntlSubdivision Component
=============

A companion component to Symfony's Intl Component. This component allows for easy retrieval of a country's states/provinces
using the country's [ISO 3166-1 alpha-2] [0] code. This code is verified using Symfony's Intl library.

The Symfony Intl component is a replacement for the C intl extension. It is limited to only the "en" locale. If you want
to have access to more locales you should [install the intl PECL extension] [1].

### Usage:

```php
// States/Provinces for the United States of America
$subdivisionsForUS = \Symfony\Component\IntlSubdivision::getSubdivision()->getStatesAndProvincesForCountry('US');
  
// States/Provinces for Canada
$subdivisionsForCA = \Symfony\Component\IntlSubdivision::getSubdivision()->getStatesAndProvincesForCountry('CA');
  
// States/Provinces for the United Arab Emirates
$subdivisionsForAE = \Symfony\Component\IntlSubdivision::getSubdivision()->getStatesAndProvincesForCountry('AE');
```


Resources
---------

  * [Documentation](https://symfony.com/doc/current/components/intl.html)
  * [Contributing](https://symfony.com/doc/current/contributing/index.html)
  * [Report issues](https://github.com/trickeyone/intl-subdivision/issues) and
    [send Pull Requests](https://github.com/trickeyone/intl-subdivision/pulls)

[0]: http://www.iso.org/iso/home/standards/country_codes.htm
[1]: http://www.php.net/manual/en/intl.setup.php
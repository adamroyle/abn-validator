# ABN and ACN validation for PHP

By [Paul Ferrett](http://www.paulferrett.com)

## Installation

    composer require ifunk/abn-validator

## Usage

```php
AbnValidator::isValidAbn('53 004 085 616'); // -> true
AbnValidator::isValidAbn('0'); // -> false
AbnValidator::isValidAcn('005 749 986'); // -> true
AbnValidator::isValidAcn('53 004 085 616'); // -> false  (that's an ABN!)
AbnValidator::isValidAbnOrAcn('53 004 085 616'); // -> true
AbnValidator::isValidAbnOrAcn('005 749 986'); // -> true
AbnValidator::isValidAbnOrAcn('0'); // -> false
```

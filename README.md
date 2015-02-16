# PHPStorm Code Style

This PHPStorm Code Style follows the [PSR-1 coding standard] (http://www.php-fig.org/psr/psr-1/) and [PSR-2 coding style] (http://www.php-fig.org/psr/psr-2/) with a few modifications specific to our company's taste.


## Spaces before and after unary Not (!)

We insert a space before and after the unary Not (!). This makes for a more obvious usage of the (!) which would otherwise be easy to miss. Example:

```php
if( ! $success) {
    echo 'hello';
}
```

## Align key-value pairs

We align the key value pairs in an array.

```php
$x = [
    0   => "zero",
    123 => "one two three",
    25  => "two five"
];
```

## Class declaration

We insert a line right after the class declaration. The only reason for this is that it looks cleaner in lengthy classes (subjective).

Before:
```php
<?php

namespace Coreproc\Objects;

class User
{
    public function test()
    {
        echo 'hello';
    }
}
```

After:
```php
<?php

namespace Coreproc\Objects;

class User
{

    public function test()
    {
        echo 'hello';
    }

}
```


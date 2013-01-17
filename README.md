exceptions
==========

A repository to create and return exceptions according to an ini file.

# Usage

You can include this in your PHP project through the PHP [composer](http://getcomposer.org).
Using TDTExceptions is very easy:

```php
throw new TDTException(452,array(parameter1, parameter2));
```

This will cause the class TDTException look in the exceptions.ini file. From that file it will extract the necessary information such documentation, and message to create a nice exception.
In the exceptions.ini file you can see the message can accept parameters. These are the parameters you pass along with the constructor in the array as second parameter. In the ini file you can
address these parameters by $1,$2,...
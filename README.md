# ZF3-BarLogger, integrated [Tracy Dumper](https://github.com/nette/tracy) from [Nette framework](https://nette.org/) in Zend Framework 3 Developer Tools

-----


**BarLogger** is collector to zend developer tools bar some data do dump.

# Module installation
  1. `cd my/project/directory`
  2. create a `composer.json` file with following contents:

     ```json
     {
         "require": {
             "renat-magadiev/zf3-bar-logger": "^1.0"
         }
     }
     ```
  3. install composer via `curl -s http://getcomposer.org/installer | php` (on windows, download
     http://getcomposer.org/installer and execute it with PHP)
  4. run `php composer.phar install`
  5. open `my/project/directory/configs/modules.config.php` and add the following key :

     ```php
     'BarLogger',
     ```

# Features

### Dump data to Zend Developer Tools 


##### Usage :
You can use `\BarLogger\Collector\DebugCollector::barDump` to dump data to bar
```php
\BarLogger\Collector\DebugCollector::barDump($var, $title, $options);
```

There is also a shortcut via global function loaded by composer so you can call anywhere:
```php
barDump($var, $title, $options);
```


# License

**renat-magadiev/zf3-bar-logger** is licensed under the MIT License - See the [LICENSE](LICENSE.md) file for details.

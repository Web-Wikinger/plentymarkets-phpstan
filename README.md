# plentymarkets-phpstan
Configuration of PHPStan for plentymarkets plugins

## Links
https://phpstan.org/


## 1. Add PHPStan to Project
add this file to root of the project



```Add to composer.json
{
   "require-dev": {
       "phpstan/phpstan": "^1.6"
   },
   "require": {
       "friendsofphp/php-cs-fixer": "^3.8"
   }
}

``` 

run composer install 

```Add configuration to phpstan.neon

parameters:
	level: 1
	paths:
		- src
		- resources

```
## Test the Code locally
```
php vendor/bin/phpstan analyse src/ --level=1
```

Level 1- 10, 1 ist soft , 10 is strict testing

# php-whois

PHP class to retrieve WHOIS information.

## Example of usage

```php

<?php

$domain = 'uol.com.br';

$whois = new Phois\Whois\Whois($domain);

$whois_answer = $whois->info();
$nsServers = $whois->getNsServers();

echo $whois_answer;

if ($whois->isAvailable()) {
    echo "Domain is available\n";
} else {
    echo "Domain is registered\n";
}

```

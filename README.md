# BehalfSignature

A class to handle signing of Behalf API v3+ requests

```
$userAgent = 'Mozilla 5.0';
$uri = '/api/account';
$body = '{"firstname": "me"}';
$query = 'query=value';
$privateKey = sha1('test key');

$signature = new CreateSignature($userAgent, $uri, $body, $query, $privateKey);
$signature->generateHash();
```

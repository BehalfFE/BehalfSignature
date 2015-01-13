# BehalfSignature

A class to handle signing of Behalf API v3+ requests

```
$userAgent = 'Mozilla 5.0';
$uri = '/api/account';
$body = '{"firstname": "me"}';
$query = 'query=value';
$privateKey = <Private Key provided by Behalf>;

$signature = new CreateSignature($userAgent, $uri, $body, $query, $privateKey);
$signature->generateHash();
```

# BehalfSignature

A class to handle signing of Behalf API v3+ requests

```
$userAgent = 'Mozilla 5.0'; /// User-Agent header value
$uri = '/api/account'; /// path part of the request URL
$body = '{"firstname": "me"}'; /// body of the request
$query = 'query=value'; /// query part of the request URL
$privateKey = <Private Key provided by Behalf>;

$signature = new CreateSignature($userAgent, $uri, $body, $query, $privateKey);
$signature->generateHash();
```

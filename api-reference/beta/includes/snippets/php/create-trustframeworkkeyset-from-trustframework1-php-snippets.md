---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW VERSION OF THE SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new TrustFrameworkKeySet();
$requestBody->setId('keyset1');

$result = $graphServiceClient->trustFramework()->keySets()->post($requestBody)->wait();

```
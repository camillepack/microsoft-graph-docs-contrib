---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = IdentityProviderBaseRequestBuilder.IdentityProviderBaseRequestBuilderGetQueryParameters(
		filter = "domains/any(x: x/id eq 'contoso.com')",
)

request_configuration = IdentityProviderBaseRequestBuilder.IdentityProviderBaseRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.directory.federation_configurations.by_federation_configuration_id('identityProviderBase-id').get(request_configuration = request_configuration)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = ExternalItem(
	acl = [
		Acl(
			type = AclType.User,
			value = "e811976d-83df-4cbd-8b9b-5215b18aa874",
			access_type = AccessType.Grant,
		),
		Acl(
			type = AclType.ExternalGroup,
			value = "14m1b9c38qe647f6a",
			access_type = AccessType.Deny,
		),
	]
	properties = Properties(
		additional_data = {
				"title" : "Error in the payment gateway",
				"priority" : 1,
				"assignee" : "john@contoso.com",
		}
	),
	content = ExternalItemContent(
		value = "Error in payment gateway...",
		type = ExternalItemContentType.Text,
	),
)

result = await graph_client.external.connections.by_connection_id('externalConnection-id').items.by_item_id('externalItem-id').put(request_body = request_body)


```
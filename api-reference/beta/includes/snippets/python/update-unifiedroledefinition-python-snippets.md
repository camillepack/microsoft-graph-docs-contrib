---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = UnifiedRoleDefinition(
	description = "Update basic properties of application registrations",
	display_name = "Application Registration Support Administrator",
	role_permissions = [
		UnifiedRolePermission(
			allowed_resource_actions = [
				"microsoft.directory/applications/basic/read",
			]
		),
	]
)

result = await graph_client.role_management.directory.role_definitions.by_role_definition_id('unifiedRoleDefinition-id').patch(request_body = request_body)


```
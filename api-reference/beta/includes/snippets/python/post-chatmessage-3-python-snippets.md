---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = ChatMessage(
	subject = None,
	body = ItemBody(
		content_type = BodyType.Html,
		content = "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>",
	),
	attachments = [
		ChatMessageAttachment(
			id = "74d20c7f34aa4a7fb74e2b30004247c5",
			content_type = "application/vnd.microsoft.card.thumbnail",
			content_url = None,
			content = "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\r\nAnd a <a href=\"http://microsoft.com/\">hyperlink</a>. <br>\r\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
			name = None,
			thumbnail_url = None,
		),
	]
)

result = await graph_client.teams.by_team_id('team-id').channels.by_channel_id('channel-id').messages.post(request_body = request_body)


```
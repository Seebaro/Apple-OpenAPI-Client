# WebhookPingResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**WebhookPing**](WebhookPing.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.webhook_ping_response import WebhookPingResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookPingResponse from a JSON string
webhook_ping_response_instance = WebhookPingResponse.from_json(json)
# print the JSON string representation of the object
print(WebhookPingResponse.to_json())

# convert the object into a dict
webhook_ping_response_dict = webhook_ping_response_instance.to_dict()
# create an instance of WebhookPingResponse from a dict
webhook_ping_response_from_dict = WebhookPingResponse.from_dict(webhook_ping_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WebhookPingCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**WebhookPingCreateRequestData**](WebhookPingCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.webhook_ping_create_request import WebhookPingCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookPingCreateRequest from a JSON string
webhook_ping_create_request_instance = WebhookPingCreateRequest.from_json(json)
# print the JSON string representation of the object
print(WebhookPingCreateRequest.to_json())

# convert the object into a dict
webhook_ping_create_request_dict = webhook_ping_create_request_instance.to_dict()
# create an instance of WebhookPingCreateRequest from a dict
webhook_ping_create_request_from_dict = WebhookPingCreateRequest.from_dict(webhook_ping_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



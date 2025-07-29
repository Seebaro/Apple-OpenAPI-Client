# WebhookPingCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**WebhookPingCreateRequestDataRelationships**](WebhookPingCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.webhook_ping_create_request_data import WebhookPingCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookPingCreateRequestData from a JSON string
webhook_ping_create_request_data_instance = WebhookPingCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(WebhookPingCreateRequestData.to_json())

# convert the object into a dict
webhook_ping_create_request_data_dict = webhook_ping_create_request_data_instance.to_dict()
# create an instance of WebhookPingCreateRequestData from a dict
webhook_ping_create_request_data_from_dict = WebhookPingCreateRequestData.from_dict(webhook_ping_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



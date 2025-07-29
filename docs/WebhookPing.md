# WebhookPing


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_ping import WebhookPing

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookPing from a JSON string
webhook_ping_instance = WebhookPing.from_json(json)
# print the JSON string representation of the object
print(WebhookPing.to_json())

# convert the object into a dict
webhook_ping_dict = webhook_ping_instance.to_dict()
# create an instance of WebhookPing from a dict
webhook_ping_from_dict = WebhookPing.from_dict(webhook_ping_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



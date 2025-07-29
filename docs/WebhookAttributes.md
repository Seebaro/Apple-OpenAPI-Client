# WebhookAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**event_types** | [**List[WebhookEventType]**](WebhookEventType.md) |  | [optional] 
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.webhook_attributes import WebhookAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookAttributes from a JSON string
webhook_attributes_instance = WebhookAttributes.from_json(json)
# print the JSON string representation of the object
print(WebhookAttributes.to_json())

# convert the object into a dict
webhook_attributes_dict = webhook_attributes_instance.to_dict()
# create an instance of WebhookAttributes from a dict
webhook_attributes_from_dict = WebhookAttributes.from_dict(webhook_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



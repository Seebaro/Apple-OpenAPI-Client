# WebhookEventAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_type** | [**WebhookEventType**](WebhookEventType.md) |  | [optional] 
**payload** | **str** |  | [optional] 
**ping** | **bool** |  | [optional] 
**created_date** | **datetime** |  | [optional] 

## Example

```python
from openapi_client.models.webhook_event_attributes import WebhookEventAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEventAttributes from a JSON string
webhook_event_attributes_instance = WebhookEventAttributes.from_json(json)
# print the JSON string representation of the object
print(WebhookEventAttributes.to_json())

# convert the object into a dict
webhook_event_attributes_dict = webhook_event_attributes_instance.to_dict()
# create an instance of WebhookEventAttributes from a dict
webhook_event_attributes_from_dict = WebhookEventAttributes.from_dict(webhook_event_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



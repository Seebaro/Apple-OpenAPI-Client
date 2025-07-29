# WebhookCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | 
**event_types** | [**List[WebhookEventType]**](WebhookEventType.md) |  | 
**name** | **str** |  | 
**secret** | **str** |  | 
**url** | **str** |  | 

## Example

```python
from openapi_client.models.webhook_create_request_data_attributes import WebhookCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookCreateRequestDataAttributes from a JSON string
webhook_create_request_data_attributes_instance = WebhookCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(WebhookCreateRequestDataAttributes.to_json())

# convert the object into a dict
webhook_create_request_data_attributes_dict = webhook_create_request_data_attributes_instance.to_dict()
# create an instance of WebhookCreateRequestDataAttributes from a dict
webhook_create_request_data_attributes_from_dict = WebhookCreateRequestDataAttributes.from_dict(webhook_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



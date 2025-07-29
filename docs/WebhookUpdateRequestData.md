# WebhookUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**WebhookUpdateRequestDataAttributes**](WebhookUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_update_request_data import WebhookUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookUpdateRequestData from a JSON string
webhook_update_request_data_instance = WebhookUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(WebhookUpdateRequestData.to_json())

# convert the object into a dict
webhook_update_request_data_dict = webhook_update_request_data_instance.to_dict()
# create an instance of WebhookUpdateRequestData from a dict
webhook_update_request_data_from_dict = WebhookUpdateRequestData.from_dict(webhook_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



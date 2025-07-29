# WebhookDeliveryAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_date** | **datetime** |  | [optional] 
**delivery_state** | **str** |  | [optional] 
**error_message** | **str** |  | [optional] 
**redelivery** | **bool** |  | [optional] 
**sent_date** | **datetime** |  | [optional] 
**request** | [**BetaAppClipInvocationAttributes**](BetaAppClipInvocationAttributes.md) |  | [optional] 
**response** | [**WebhookDeliveryAttributesResponse**](WebhookDeliveryAttributesResponse.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_delivery_attributes import WebhookDeliveryAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryAttributes from a JSON string
webhook_delivery_attributes_instance = WebhookDeliveryAttributes.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryAttributes.to_json())

# convert the object into a dict
webhook_delivery_attributes_dict = webhook_delivery_attributes_instance.to_dict()
# create an instance of WebhookDeliveryAttributes from a dict
webhook_delivery_attributes_from_dict = WebhookDeliveryAttributes.from_dict(webhook_delivery_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



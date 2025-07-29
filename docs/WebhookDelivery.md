# WebhookDelivery


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**WebhookDeliveryAttributes**](WebhookDeliveryAttributes.md) |  | [optional] 
**relationships** | [**WebhookDeliveryRelationships**](WebhookDeliveryRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_delivery import WebhookDelivery

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDelivery from a JSON string
webhook_delivery_instance = WebhookDelivery.from_json(json)
# print the JSON string representation of the object
print(WebhookDelivery.to_json())

# convert the object into a dict
webhook_delivery_dict = webhook_delivery_instance.to_dict()
# create an instance of WebhookDelivery from a dict
webhook_delivery_from_dict = WebhookDelivery.from_dict(webhook_delivery_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



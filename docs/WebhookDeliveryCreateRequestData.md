# WebhookDeliveryCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**WebhookDeliveryCreateRequestDataRelationships**](WebhookDeliveryCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.webhook_delivery_create_request_data import WebhookDeliveryCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryCreateRequestData from a JSON string
webhook_delivery_create_request_data_instance = WebhookDeliveryCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryCreateRequestData.to_json())

# convert the object into a dict
webhook_delivery_create_request_data_dict = webhook_delivery_create_request_data_instance.to_dict()
# create an instance of WebhookDeliveryCreateRequestData from a dict
webhook_delivery_create_request_data_from_dict = WebhookDeliveryCreateRequestData.from_dict(webhook_delivery_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



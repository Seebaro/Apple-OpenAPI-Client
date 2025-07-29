# WebhookDeliveryCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**WebhookDeliveryCreateRequestData**](WebhookDeliveryCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.webhook_delivery_create_request import WebhookDeliveryCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryCreateRequest from a JSON string
webhook_delivery_create_request_instance = WebhookDeliveryCreateRequest.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryCreateRequest.to_json())

# convert the object into a dict
webhook_delivery_create_request_dict = webhook_delivery_create_request_instance.to_dict()
# create an instance of WebhookDeliveryCreateRequest from a dict
webhook_delivery_create_request_from_dict = WebhookDeliveryCreateRequest.from_dict(webhook_delivery_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



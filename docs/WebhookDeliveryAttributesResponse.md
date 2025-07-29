# WebhookDeliveryAttributesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_status_code** | **int** |  | [optional] 
**body** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.webhook_delivery_attributes_response import WebhookDeliveryAttributesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryAttributesResponse from a JSON string
webhook_delivery_attributes_response_instance = WebhookDeliveryAttributesResponse.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryAttributesResponse.to_json())

# convert the object into a dict
webhook_delivery_attributes_response_dict = webhook_delivery_attributes_response_instance.to_dict()
# create an instance of WebhookDeliveryAttributesResponse from a dict
webhook_delivery_attributes_response_from_dict = WebhookDeliveryAttributesResponse.from_dict(webhook_delivery_attributes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



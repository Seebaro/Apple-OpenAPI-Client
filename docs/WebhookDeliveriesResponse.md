# WebhookDeliveriesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WebhookDelivery]**](WebhookDelivery.md) |  | 
**included** | [**List[WebhookEvent]**](WebhookEvent.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_deliveries_response import WebhookDeliveriesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveriesResponse from a JSON string
webhook_deliveries_response_instance = WebhookDeliveriesResponse.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveriesResponse.to_json())

# convert the object into a dict
webhook_deliveries_response_dict = webhook_deliveries_response_instance.to_dict()
# create an instance of WebhookDeliveriesResponse from a dict
webhook_deliveries_response_from_dict = WebhookDeliveriesResponse.from_dict(webhook_deliveries_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# WebhookDeliveriesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WebhookDeliveryCreateRequestDataRelationshipsTemplateData]**](WebhookDeliveryCreateRequestDataRelationshipsTemplateData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.webhook_deliveries_linkages_response import WebhookDeliveriesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveriesLinkagesResponse from a JSON string
webhook_deliveries_linkages_response_instance = WebhookDeliveriesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveriesLinkagesResponse.to_json())

# convert the object into a dict
webhook_deliveries_linkages_response_dict = webhook_deliveries_linkages_response_instance.to_dict()
# create an instance of WebhookDeliveriesLinkagesResponse from a dict
webhook_deliveries_linkages_response_from_dict = WebhookDeliveriesLinkagesResponse.from_dict(webhook_deliveries_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



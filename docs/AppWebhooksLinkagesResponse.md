# AppWebhooksLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[WebhookPingCreateRequestDataRelationshipsWebhookData]**](WebhookPingCreateRequestDataRelationshipsWebhookData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_webhooks_linkages_response import AppWebhooksLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppWebhooksLinkagesResponse from a JSON string
app_webhooks_linkages_response_instance = AppWebhooksLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppWebhooksLinkagesResponse.to_json())

# convert the object into a dict
app_webhooks_linkages_response_dict = app_webhooks_linkages_response_instance.to_dict()
# create an instance of AppWebhooksLinkagesResponse from a dict
app_webhooks_linkages_response_from_dict = AppWebhooksLinkagesResponse.from_dict(app_webhooks_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



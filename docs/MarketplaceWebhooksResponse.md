# MarketplaceWebhooksResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[MarketplaceWebhook]**](MarketplaceWebhook.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.marketplace_webhooks_response import MarketplaceWebhooksResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhooksResponse from a JSON string
marketplace_webhooks_response_instance = MarketplaceWebhooksResponse.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhooksResponse.to_json())

# convert the object into a dict
marketplace_webhooks_response_dict = marketplace_webhooks_response_instance.to_dict()
# create an instance of MarketplaceWebhooksResponse from a dict
marketplace_webhooks_response_from_dict = MarketplaceWebhooksResponse.from_dict(marketplace_webhooks_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



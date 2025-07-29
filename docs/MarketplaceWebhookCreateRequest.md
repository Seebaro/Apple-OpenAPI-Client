# MarketplaceWebhookCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MarketplaceWebhookCreateRequestData**](MarketplaceWebhookCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.marketplace_webhook_create_request import MarketplaceWebhookCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookCreateRequest from a JSON string
marketplace_webhook_create_request_instance = MarketplaceWebhookCreateRequest.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookCreateRequest.to_json())

# convert the object into a dict
marketplace_webhook_create_request_dict = marketplace_webhook_create_request_instance.to_dict()
# create an instance of MarketplaceWebhookCreateRequest from a dict
marketplace_webhook_create_request_from_dict = MarketplaceWebhookCreateRequest.from_dict(marketplace_webhook_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MarketplaceWebhookUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MarketplaceWebhookUpdateRequestData**](MarketplaceWebhookUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.marketplace_webhook_update_request import MarketplaceWebhookUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookUpdateRequest from a JSON string
marketplace_webhook_update_request_instance = MarketplaceWebhookUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookUpdateRequest.to_json())

# convert the object into a dict
marketplace_webhook_update_request_dict = marketplace_webhook_update_request_instance.to_dict()
# create an instance of MarketplaceWebhookUpdateRequest from a dict
marketplace_webhook_update_request_from_dict = MarketplaceWebhookUpdateRequest.from_dict(marketplace_webhook_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



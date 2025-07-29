# MarketplaceWebhookResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MarketplaceWebhook**](MarketplaceWebhook.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.marketplace_webhook_response import MarketplaceWebhookResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookResponse from a JSON string
marketplace_webhook_response_instance = MarketplaceWebhookResponse.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookResponse.to_json())

# convert the object into a dict
marketplace_webhook_response_dict = marketplace_webhook_response_instance.to_dict()
# create an instance of MarketplaceWebhookResponse from a dict
marketplace_webhook_response_from_dict = MarketplaceWebhookResponse.from_dict(marketplace_webhook_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



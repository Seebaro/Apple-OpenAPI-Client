# MarketplaceWebhook


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**MarketplaceWebhookAttributes**](MarketplaceWebhookAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.marketplace_webhook import MarketplaceWebhook

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhook from a JSON string
marketplace_webhook_instance = MarketplaceWebhook.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhook.to_json())

# convert the object into a dict
marketplace_webhook_dict = marketplace_webhook_instance.to_dict()
# create an instance of MarketplaceWebhook from a dict
marketplace_webhook_from_dict = MarketplaceWebhook.from_dict(marketplace_webhook_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MarketplaceWebhookAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**endpoint_url** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.marketplace_webhook_attributes import MarketplaceWebhookAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookAttributes from a JSON string
marketplace_webhook_attributes_instance = MarketplaceWebhookAttributes.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookAttributes.to_json())

# convert the object into a dict
marketplace_webhook_attributes_dict = marketplace_webhook_attributes_instance.to_dict()
# create an instance of MarketplaceWebhookAttributes from a dict
marketplace_webhook_attributes_from_dict = MarketplaceWebhookAttributes.from_dict(marketplace_webhook_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



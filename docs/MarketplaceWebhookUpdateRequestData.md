# MarketplaceWebhookUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**MarketplaceWebhookUpdateRequestDataAttributes**](MarketplaceWebhookUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.marketplace_webhook_update_request_data import MarketplaceWebhookUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookUpdateRequestData from a JSON string
marketplace_webhook_update_request_data_instance = MarketplaceWebhookUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookUpdateRequestData.to_json())

# convert the object into a dict
marketplace_webhook_update_request_data_dict = marketplace_webhook_update_request_data_instance.to_dict()
# create an instance of MarketplaceWebhookUpdateRequestData from a dict
marketplace_webhook_update_request_data_from_dict = MarketplaceWebhookUpdateRequestData.from_dict(marketplace_webhook_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MarketplaceWebhookCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**MarketplaceWebhookCreateRequestDataAttributes**](MarketplaceWebhookCreateRequestDataAttributes.md) |  | 

## Example

```python
from openapi_client.models.marketplace_webhook_create_request_data import MarketplaceWebhookCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookCreateRequestData from a JSON string
marketplace_webhook_create_request_data_instance = MarketplaceWebhookCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookCreateRequestData.to_json())

# convert the object into a dict
marketplace_webhook_create_request_data_dict = marketplace_webhook_create_request_data_instance.to_dict()
# create an instance of MarketplaceWebhookCreateRequestData from a dict
marketplace_webhook_create_request_data_from_dict = MarketplaceWebhookCreateRequestData.from_dict(marketplace_webhook_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



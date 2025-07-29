# MarketplaceWebhookCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**endpoint_url** | **str** |  | 
**secret** | **str** |  | 

## Example

```python
from openapi_client.models.marketplace_webhook_create_request_data_attributes import MarketplaceWebhookCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookCreateRequestDataAttributes from a JSON string
marketplace_webhook_create_request_data_attributes_instance = MarketplaceWebhookCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookCreateRequestDataAttributes.to_json())

# convert the object into a dict
marketplace_webhook_create_request_data_attributes_dict = marketplace_webhook_create_request_data_attributes_instance.to_dict()
# create an instance of MarketplaceWebhookCreateRequestDataAttributes from a dict
marketplace_webhook_create_request_data_attributes_from_dict = MarketplaceWebhookCreateRequestDataAttributes.from_dict(marketplace_webhook_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MarketplaceWebhookUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**endpoint_url** | **str** |  | [optional] 
**secret** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.marketplace_webhook_update_request_data_attributes import MarketplaceWebhookUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of MarketplaceWebhookUpdateRequestDataAttributes from a JSON string
marketplace_webhook_update_request_data_attributes_instance = MarketplaceWebhookUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(MarketplaceWebhookUpdateRequestDataAttributes.to_json())

# convert the object into a dict
marketplace_webhook_update_request_data_attributes_dict = marketplace_webhook_update_request_data_attributes_instance.to_dict()
# create an instance of MarketplaceWebhookUpdateRequestDataAttributes from a dict
marketplace_webhook_update_request_data_attributes_from_dict = MarketplaceWebhookUpdateRequestDataAttributes.from_dict(marketplace_webhook_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



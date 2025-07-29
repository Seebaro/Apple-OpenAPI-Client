# SubscriptionUpdateRequestDataRelationshipsPrices


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SubscriptionRelationshipsPricesDataInner]**](SubscriptionRelationshipsPricesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_update_request_data_relationships_prices import SubscriptionUpdateRequestDataRelationshipsPrices

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionUpdateRequestDataRelationshipsPrices from a JSON string
subscription_update_request_data_relationships_prices_instance = SubscriptionUpdateRequestDataRelationshipsPrices.from_json(json)
# print the JSON string representation of the object
print(SubscriptionUpdateRequestDataRelationshipsPrices.to_json())

# convert the object into a dict
subscription_update_request_data_relationships_prices_dict = subscription_update_request_data_relationships_prices_instance.to_dict()
# create an instance of SubscriptionUpdateRequestDataRelationshipsPrices from a dict
subscription_update_request_data_relationships_prices_from_dict = SubscriptionUpdateRequestDataRelationshipsPrices.from_dict(subscription_update_request_data_relationships_prices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



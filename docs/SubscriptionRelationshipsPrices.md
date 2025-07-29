# SubscriptionRelationshipsPrices


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[SubscriptionRelationshipsPricesDataInner]**](SubscriptionRelationshipsPricesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_relationships_prices import SubscriptionRelationshipsPrices

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionRelationshipsPrices from a JSON string
subscription_relationships_prices_instance = SubscriptionRelationshipsPrices.from_json(json)
# print the JSON string representation of the object
print(SubscriptionRelationshipsPrices.to_json())

# convert the object into a dict
subscription_relationships_prices_dict = subscription_relationships_prices_instance.to_dict()
# create an instance of SubscriptionRelationshipsPrices from a dict
subscription_relationships_prices_from_dict = SubscriptionRelationshipsPrices.from_dict(subscription_relationships_prices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# InAppPurchasePriceRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**in_app_purchase_price_point** | [**InAppPurchasePriceRelationshipsInAppPurchasePricePoint**](InAppPurchasePriceRelationshipsInAppPurchasePricePoint.md) |  | [optional] 
**territory** | [**AppPricePointV3RelationshipsTerritory**](AppPricePointV3RelationshipsTerritory.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_relationships import InAppPurchasePriceRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceRelationships from a JSON string
in_app_purchase_price_relationships_instance = InAppPurchasePriceRelationships.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceRelationships.to_json())

# convert the object into a dict
in_app_purchase_price_relationships_dict = in_app_purchase_price_relationships_instance.to_dict()
# create an instance of InAppPurchasePriceRelationships from a dict
in_app_purchase_price_relationships_from_dict = InAppPurchasePriceRelationships.from_dict(in_app_purchase_price_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# InAppPurchaseV2RelationshipsPricePoints


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[InAppPurchasePriceRelationshipsInAppPurchasePricePointData]**](InAppPurchasePriceRelationshipsInAppPurchasePricePointData.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_relationships_price_points import InAppPurchaseV2RelationshipsPricePoints

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2RelationshipsPricePoints from a JSON string
in_app_purchase_v2_relationships_price_points_instance = InAppPurchaseV2RelationshipsPricePoints.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2RelationshipsPricePoints.to_json())

# convert the object into a dict
in_app_purchase_v2_relationships_price_points_dict = in_app_purchase_v2_relationships_price_points_instance.to_dict()
# create an instance of InAppPurchaseV2RelationshipsPricePoints from a dict
in_app_purchase_v2_relationships_price_points_from_dict = InAppPurchaseV2RelationshipsPricePoints.from_dict(in_app_purchase_v2_relationships_price_points_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# InAppPurchaseV2RelationshipsPromotedPurchase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**AppRelationshipsPromotedPurchasesDataInner**](AppRelationshipsPromotedPurchasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_relationships_promoted_purchase import InAppPurchaseV2RelationshipsPromotedPurchase

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2RelationshipsPromotedPurchase from a JSON string
in_app_purchase_v2_relationships_promoted_purchase_instance = InAppPurchaseV2RelationshipsPromotedPurchase.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2RelationshipsPromotedPurchase.to_json())

# convert the object into a dict
in_app_purchase_v2_relationships_promoted_purchase_dict = in_app_purchase_v2_relationships_promoted_purchase_instance.to_dict()
# create an instance of InAppPurchaseV2RelationshipsPromotedPurchase from a dict
in_app_purchase_v2_relationships_promoted_purchase_from_dict = InAppPurchaseV2RelationshipsPromotedPurchase.from_dict(in_app_purchase_v2_relationships_promoted_purchase_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



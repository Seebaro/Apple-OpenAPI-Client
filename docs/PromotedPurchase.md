# PromotedPurchase


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**PromotedPurchaseAttributes**](PromotedPurchaseAttributes.md) |  | [optional] 
**relationships** | [**PromotedPurchaseRelationships**](PromotedPurchaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchase import PromotedPurchase

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchase from a JSON string
promoted_purchase_instance = PromotedPurchase.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchase.to_json())

# convert the object into a dict
promoted_purchase_dict = promoted_purchase_instance.to_dict()
# create an instance of PromotedPurchase from a dict
promoted_purchase_from_dict = PromotedPurchase.from_dict(promoted_purchase_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



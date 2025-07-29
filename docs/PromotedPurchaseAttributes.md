# PromotedPurchaseAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**visible_for_all_users** | **bool** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchase_attributes import PromotedPurchaseAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseAttributes from a JSON string
promoted_purchase_attributes_instance = PromotedPurchaseAttributes.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseAttributes.to_json())

# convert the object into a dict
promoted_purchase_attributes_dict = promoted_purchase_attributes_instance.to_dict()
# create an instance of PromotedPurchaseAttributes from a dict
promoted_purchase_attributes_from_dict = PromotedPurchaseAttributes.from_dict(promoted_purchase_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



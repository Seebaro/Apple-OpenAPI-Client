# InAppPurchaseV2Attributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**product_id** | **str** |  | [optional] 
**in_app_purchase_type** | [**InAppPurchaseType**](InAppPurchaseType.md) |  | [optional] 
**state** | [**InAppPurchaseState**](InAppPurchaseState.md) |  | [optional] 
**review_note** | **str** |  | [optional] 
**family_sharable** | **bool** |  | [optional] 
**content_hosting** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_attributes import InAppPurchaseV2Attributes

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2Attributes from a JSON string
in_app_purchase_v2_attributes_instance = InAppPurchaseV2Attributes.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2Attributes.to_json())

# convert the object into a dict
in_app_purchase_v2_attributes_dict = in_app_purchase_v2_attributes_instance.to_dict()
# create an instance of InAppPurchaseV2Attributes from a dict
in_app_purchase_v2_attributes_from_dict = InAppPurchaseV2Attributes.from_dict(in_app_purchase_v2_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



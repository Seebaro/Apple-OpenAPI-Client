# InAppPurchasesV2ResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseImageAttributes**](InAppPurchaseImageAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseImageRelationships**](InAppPurchaseImageRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchases_v2_response_included_inner import InAppPurchasesV2ResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasesV2ResponseIncludedInner from a JSON string
in_app_purchases_v2_response_included_inner_instance = InAppPurchasesV2ResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasesV2ResponseIncludedInner.to_json())

# convert the object into a dict
in_app_purchases_v2_response_included_inner_dict = in_app_purchases_v2_response_included_inner_instance.to_dict()
# create an instance of InAppPurchasesV2ResponseIncludedInner from a dict
in_app_purchases_v2_response_included_inner_from_dict = InAppPurchasesV2ResponseIncludedInner.from_dict(in_app_purchases_v2_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# InAppPurchaseV2PromotedPurchaseLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsPromotedPurchasesDataInner**](AppRelationshipsPromotedPurchasesDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_v2_promoted_purchase_linkage_response import InAppPurchaseV2PromotedPurchaseLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2PromotedPurchaseLinkageResponse from a JSON string
in_app_purchase_v2_promoted_purchase_linkage_response_instance = InAppPurchaseV2PromotedPurchaseLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2PromotedPurchaseLinkageResponse.to_json())

# convert the object into a dict
in_app_purchase_v2_promoted_purchase_linkage_response_dict = in_app_purchase_v2_promoted_purchase_linkage_response_instance.to_dict()
# create an instance of InAppPurchaseV2PromotedPurchaseLinkageResponse from a dict
in_app_purchase_v2_promoted_purchase_linkage_response_from_dict = InAppPurchaseV2PromotedPurchaseLinkageResponse.from_dict(in_app_purchase_v2_promoted_purchase_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# PromotedPurchaseCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AccessibilityDeclarationCreateRequestDataRelationshipsApp**](AccessibilityDeclarationCreateRequestDataRelationshipsApp.md) |  | 
**in_app_purchase_v2** | [**InAppPurchaseAppStoreReviewScreenshotRelationshipsInAppPurchaseV2**](InAppPurchaseAppStoreReviewScreenshotRelationshipsInAppPurchaseV2.md) |  | [optional] 
**subscription** | [**PromotedPurchaseRelationshipsSubscription**](PromotedPurchaseRelationshipsSubscription.md) |  | [optional] 

## Example

```python
from openapi_client.models.promoted_purchase_create_request_data_relationships import PromotedPurchaseCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of PromotedPurchaseCreateRequestDataRelationships from a JSON string
promoted_purchase_create_request_data_relationships_instance = PromotedPurchaseCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(PromotedPurchaseCreateRequestDataRelationships.to_json())

# convert the object into a dict
promoted_purchase_create_request_data_relationships_dict = promoted_purchase_create_request_data_relationships_instance.to_dict()
# create an instance of PromotedPurchaseCreateRequestDataRelationships from a dict
promoted_purchase_create_request_data_relationships_from_dict = PromotedPurchaseCreateRequestDataRelationships.from_dict(promoted_purchase_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# InAppPurchasePriceInlineCreateRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**in_app_purchase_v2** | [**InAppPurchaseAppStoreReviewScreenshotRelationshipsInAppPurchaseV2**](InAppPurchaseAppStoreReviewScreenshotRelationshipsInAppPurchaseV2.md) |  | [optional] 
**in_app_purchase_price_point** | [**InAppPurchasePriceRelationshipsInAppPurchasePricePoint**](InAppPurchasePriceRelationshipsInAppPurchasePricePoint.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_price_inline_create_relationships import InAppPurchasePriceInlineCreateRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasePriceInlineCreateRelationships from a JSON string
in_app_purchase_price_inline_create_relationships_instance = InAppPurchasePriceInlineCreateRelationships.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasePriceInlineCreateRelationships.to_json())

# convert the object into a dict
in_app_purchase_price_inline_create_relationships_dict = in_app_purchase_price_inline_create_relationships_instance.to_dict()
# create an instance of InAppPurchasePriceInlineCreateRelationships from a dict
in_app_purchase_price_inline_create_relationships_from_dict = InAppPurchasePriceInlineCreateRelationships.from_dict(in_app_purchase_price_inline_create_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



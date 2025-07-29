# InAppPurchaseLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**InAppPurchaseLocalizationAttributes**](InAppPurchaseLocalizationAttributes.md) |  | [optional] 
**relationships** | [**InAppPurchaseAppStoreReviewScreenshotRelationships**](InAppPurchaseAppStoreReviewScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_localization import InAppPurchaseLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseLocalization from a JSON string
in_app_purchase_localization_instance = InAppPurchaseLocalization.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseLocalization.to_json())

# convert the object into a dict
in_app_purchase_localization_dict = in_app_purchase_localization_instance.to_dict()
# create an instance of InAppPurchaseLocalization from a dict
in_app_purchase_localization_from_dict = InAppPurchaseLocalization.from_dict(in_app_purchase_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



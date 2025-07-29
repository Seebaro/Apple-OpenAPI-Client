# InAppPurchaseLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**InAppPurchaseLocalizationCreateRequestDataAttributes**](InAppPurchaseLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**InAppPurchaseAppStoreReviewScreenshotCreateRequestDataRelationships**](InAppPurchaseAppStoreReviewScreenshotCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_localization_create_request_data import InAppPurchaseLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseLocalizationCreateRequestData from a JSON string
in_app_purchase_localization_create_request_data_instance = InAppPurchaseLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseLocalizationCreateRequestData.to_json())

# convert the object into a dict
in_app_purchase_localization_create_request_data_dict = in_app_purchase_localization_create_request_data_instance.to_dict()
# create an instance of InAppPurchaseLocalizationCreateRequestData from a dict
in_app_purchase_localization_create_request_data_from_dict = InAppPurchaseLocalizationCreateRequestData.from_dict(in_app_purchase_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# InAppPurchaseLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterActivityLocalizationUpdateRequestDataAttributes**](GameCenterActivityLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_localization_update_request_data import InAppPurchaseLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseLocalizationUpdateRequestData from a JSON string
in_app_purchase_localization_update_request_data_instance = InAppPurchaseLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseLocalizationUpdateRequestData.to_json())

# convert the object into a dict
in_app_purchase_localization_update_request_data_dict = in_app_purchase_localization_update_request_data_instance.to_dict()
# create an instance of InAppPurchaseLocalizationUpdateRequestData from a dict
in_app_purchase_localization_update_request_data_from_dict = InAppPurchaseLocalizationUpdateRequestData.from_dict(in_app_purchase_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



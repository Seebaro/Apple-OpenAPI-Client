# InAppPurchaseLocalizationAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**locale** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_localization_attributes import InAppPurchaseLocalizationAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseLocalizationAttributes from a JSON string
in_app_purchase_localization_attributes_instance = InAppPurchaseLocalizationAttributes.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseLocalizationAttributes.to_json())

# convert the object into a dict
in_app_purchase_localization_attributes_dict = in_app_purchase_localization_attributes_instance.to_dict()
# create an instance of InAppPurchaseLocalizationAttributes from a dict
in_app_purchase_localization_attributes_from_dict = InAppPurchaseLocalizationAttributes.from_dict(in_app_purchase_localization_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



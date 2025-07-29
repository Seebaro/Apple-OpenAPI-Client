# AppCustomProductPageLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCustomProductPageLocalizationAttributes**](AppCustomProductPageLocalizationAttributes.md) |  | [optional] 
**relationships** | [**AppCustomProductPageLocalizationRelationships**](AppCustomProductPageLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_localization import AppCustomProductPageLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalization from a JSON string
app_custom_product_page_localization_instance = AppCustomProductPageLocalization.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalization.to_json())

# convert the object into a dict
app_custom_product_page_localization_dict = app_custom_product_page_localization_instance.to_dict()
# create an instance of AppCustomProductPageLocalization from a dict
app_custom_product_page_localization_from_dict = AppCustomProductPageLocalization.from_dict(app_custom_product_page_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



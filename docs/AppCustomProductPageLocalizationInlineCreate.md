# AppCustomProductPageLocalizationInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**AppCustomProductPageLocalizationInlineCreateAttributes**](AppCustomProductPageLocalizationInlineCreateAttributes.md) |  | 
**relationships** | [**AppCustomProductPageLocalizationInlineCreateRelationships**](AppCustomProductPageLocalizationInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_localization_inline_create import AppCustomProductPageLocalizationInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalizationInlineCreate from a JSON string
app_custom_product_page_localization_inline_create_instance = AppCustomProductPageLocalizationInlineCreate.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalizationInlineCreate.to_json())

# convert the object into a dict
app_custom_product_page_localization_inline_create_dict = app_custom_product_page_localization_inline_create_instance.to_dict()
# create an instance of AppCustomProductPageLocalizationInlineCreate from a dict
app_custom_product_page_localization_inline_create_from_dict = AppCustomProductPageLocalizationInlineCreate.from_dict(app_custom_product_page_localization_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



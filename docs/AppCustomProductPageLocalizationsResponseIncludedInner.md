# AppCustomProductPageLocalizationsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppPreviewSetAttributes**](AppPreviewSetAttributes.md) |  | [optional] 
**relationships** | [**AppPreviewSetRelationships**](AppPreviewSetRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_localizations_response_included_inner import AppCustomProductPageLocalizationsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageLocalizationsResponseIncludedInner from a JSON string
app_custom_product_page_localizations_response_included_inner_instance = AppCustomProductPageLocalizationsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageLocalizationsResponseIncludedInner.to_json())

# convert the object into a dict
app_custom_product_page_localizations_response_included_inner_dict = app_custom_product_page_localizations_response_included_inner_instance.to_dict()
# create an instance of AppCustomProductPageLocalizationsResponseIncludedInner from a dict
app_custom_product_page_localizations_response_included_inner_from_dict = AppCustomProductPageLocalizationsResponseIncludedInner.from_dict(app_custom_product_page_localizations_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



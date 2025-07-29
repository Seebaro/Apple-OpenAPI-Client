# AppCustomProductPageVersionsResponseIncludedInner


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
from openapi_client.models.app_custom_product_page_versions_response_included_inner import AppCustomProductPageVersionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionsResponseIncludedInner from a JSON string
app_custom_product_page_versions_response_included_inner_instance = AppCustomProductPageVersionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionsResponseIncludedInner.to_json())

# convert the object into a dict
app_custom_product_page_versions_response_included_inner_dict = app_custom_product_page_versions_response_included_inner_instance.to_dict()
# create an instance of AppCustomProductPageVersionsResponseIncludedInner from a dict
app_custom_product_page_versions_response_included_inner_from_dict = AppCustomProductPageVersionsResponseIncludedInner.from_dict(app_custom_product_page_versions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



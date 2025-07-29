# AppCustomProductPageVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCustomProductPageVersionAttributes**](AppCustomProductPageVersionAttributes.md) |  | [optional] 
**relationships** | [**AppCustomProductPageVersionRelationships**](AppCustomProductPageVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_version import AppCustomProductPageVersion

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersion from a JSON string
app_custom_product_page_version_instance = AppCustomProductPageVersion.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersion.to_json())

# convert the object into a dict
app_custom_product_page_version_dict = app_custom_product_page_version_instance.to_dict()
# create an instance of AppCustomProductPageVersion from a dict
app_custom_product_page_version_from_dict = AppCustomProductPageVersion.from_dict(app_custom_product_page_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



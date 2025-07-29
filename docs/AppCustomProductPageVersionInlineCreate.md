# AppCustomProductPageVersionInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**AppCustomProductPageVersionInlineCreateAttributes**](AppCustomProductPageVersionInlineCreateAttributes.md) |  | [optional] 
**relationships** | [**AppCustomProductPageVersionInlineCreateRelationships**](AppCustomProductPageVersionInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_custom_product_page_version_inline_create import AppCustomProductPageVersionInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AppCustomProductPageVersionInlineCreate from a JSON string
app_custom_product_page_version_inline_create_instance = AppCustomProductPageVersionInlineCreate.from_json(json)
# print the JSON string representation of the object
print(AppCustomProductPageVersionInlineCreate.to_json())

# convert the object into a dict
app_custom_product_page_version_inline_create_dict = app_custom_product_page_version_inline_create_instance.to_dict()
# create an instance of AppCustomProductPageVersionInlineCreate from a dict
app_custom_product_page_version_inline_create_from_dict = AppCustomProductPageVersionInlineCreate.from_dict(app_custom_product_page_version_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



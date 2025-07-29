# AppCategoriesWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppCategory]**](AppCategory.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_categories_without_includes_response import AppCategoriesWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCategoriesWithoutIncludesResponse from a JSON string
app_categories_without_includes_response_instance = AppCategoriesWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCategoriesWithoutIncludesResponse.to_json())

# convert the object into a dict
app_categories_without_includes_response_dict = app_categories_without_includes_response_instance.to_dict()
# create an instance of AppCategoriesWithoutIncludesResponse from a dict
app_categories_without_includes_response_from_dict = AppCategoriesWithoutIncludesResponse.from_dict(app_categories_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



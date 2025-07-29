# AppCategoryWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppCategory**](AppCategory.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_category_without_includes_response import AppCategoryWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppCategoryWithoutIncludesResponse from a JSON string
app_category_without_includes_response_instance = AppCategoryWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(AppCategoryWithoutIncludesResponse.to_json())

# convert the object into a dict
app_category_without_includes_response_dict = app_category_without_includes_response_instance.to_dict()
# create an instance of AppCategoryWithoutIncludesResponse from a dict
app_category_without_includes_response_from_dict = AppCategoryWithoutIncludesResponse.from_dict(app_category_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



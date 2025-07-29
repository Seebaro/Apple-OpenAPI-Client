# AppCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppCategoryAttributes**](AppCategoryAttributes.md) |  | [optional] 
**relationships** | [**AppCategoryRelationships**](AppCategoryRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_category import AppCategory

# TODO update the JSON string below
json = "{}"
# create an instance of AppCategory from a JSON string
app_category_instance = AppCategory.from_json(json)
# print the JSON string representation of the object
print(AppCategory.to_json())

# convert the object into a dict
app_category_dict = app_category_instance.to_dict()
# create an instance of AppCategory from a dict
app_category_from_dict = AppCategory.from_dict(app_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



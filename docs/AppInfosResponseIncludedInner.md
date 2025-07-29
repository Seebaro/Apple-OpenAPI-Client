# AppInfosResponseIncludedInner


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
from openapi_client.models.app_infos_response_included_inner import AppInfosResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppInfosResponseIncludedInner from a JSON string
app_infos_response_included_inner_instance = AppInfosResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppInfosResponseIncludedInner.to_json())

# convert the object into a dict
app_infos_response_included_inner_dict = app_infos_response_included_inner_instance.to_dict()
# create an instance of AppInfosResponseIncludedInner from a dict
app_infos_response_included_inner_from_dict = AppInfosResponseIncludedInner.from_dict(app_infos_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



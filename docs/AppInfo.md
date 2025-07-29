# AppInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppInfoAttributes**](AppInfoAttributes.md) |  | [optional] 
**relationships** | [**AppInfoRelationships**](AppInfoRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_info import AppInfo

# TODO update the JSON string below
json = "{}"
# create an instance of AppInfo from a JSON string
app_info_instance = AppInfo.from_json(json)
# print the JSON string representation of the object
print(AppInfo.to_json())

# convert the object into a dict
app_info_dict = app_info_instance.to_dict()
# create an instance of AppInfo from a dict
app_info_from_dict = AppInfo.from_dict(app_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



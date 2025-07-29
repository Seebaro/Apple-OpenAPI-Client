# AppClipDefaultExperienceUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipDefaultExperienceAttributes**](AppClipDefaultExperienceAttributes.md) |  | [optional] 
**relationships** | [**AppClipDefaultExperienceUpdateRequestDataRelationships**](AppClipDefaultExperienceUpdateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_default_experience_update_request_data import AppClipDefaultExperienceUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipDefaultExperienceUpdateRequestData from a JSON string
app_clip_default_experience_update_request_data_instance = AppClipDefaultExperienceUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppClipDefaultExperienceUpdateRequestData.to_json())

# convert the object into a dict
app_clip_default_experience_update_request_data_dict = app_clip_default_experience_update_request_data_instance.to_dict()
# create an instance of AppClipDefaultExperienceUpdateRequestData from a dict
app_clip_default_experience_update_request_data_from_dict = AppClipDefaultExperienceUpdateRequestData.from_dict(app_clip_default_experience_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



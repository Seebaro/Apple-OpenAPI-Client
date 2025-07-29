# AppClipAdvancedExperienceUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipAdvancedExperienceUpdateRequestDataAttributes**](AppClipAdvancedExperienceUpdateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**AppClipAdvancedExperienceUpdateRequestDataRelationships**](AppClipAdvancedExperienceUpdateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clip_advanced_experience_update_request_data import AppClipAdvancedExperienceUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipAdvancedExperienceUpdateRequestData from a JSON string
app_clip_advanced_experience_update_request_data_instance = AppClipAdvancedExperienceUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppClipAdvancedExperienceUpdateRequestData.to_json())

# convert the object into a dict
app_clip_advanced_experience_update_request_data_dict = app_clip_advanced_experience_update_request_data_instance.to_dict()
# create an instance of AppClipAdvancedExperienceUpdateRequestData from a dict
app_clip_advanced_experience_update_request_data_from_dict = AppClipAdvancedExperienceUpdateRequestData.from_dict(app_clip_advanced_experience_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



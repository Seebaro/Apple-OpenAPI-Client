# AppClipsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppClipDefaultExperienceAttributes**](AppClipDefaultExperienceAttributes.md) |  | [optional] 
**relationships** | [**AppClipDefaultExperienceRelationships**](AppClipDefaultExperienceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clips_response_included_inner import AppClipsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipsResponseIncludedInner from a JSON string
app_clips_response_included_inner_instance = AppClipsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppClipsResponseIncludedInner.to_json())

# convert the object into a dict
app_clips_response_included_inner_dict = app_clips_response_included_inner_instance.to_dict()
# create an instance of AppClipsResponseIncludedInner from a dict
app_clips_response_included_inner_from_dict = AppClipsResponseIncludedInner.from_dict(app_clips_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



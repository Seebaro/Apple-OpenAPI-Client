# AppClipResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClip**](AppClip.md) |  | 
**included** | [**List[AppClipsResponseIncludedInner]**](AppClipsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_clip_response import AppClipResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipResponse from a JSON string
app_clip_response_instance = AppClipResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipResponse.to_json())

# convert the object into a dict
app_clip_response_dict = app_clip_response_instance.to_dict()
# create an instance of AppClipResponse from a dict
app_clip_response_from_dict = AppClipResponse.from_dict(app_clip_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



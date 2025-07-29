# AppMediaVideoState


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**errors** | [**List[AppMediaStateError]**](AppMediaStateError.md) |  | [optional] 
**warnings** | [**List[AppMediaStateError]**](AppMediaStateError.md) |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.app_media_video_state import AppMediaVideoState

# TODO update the JSON string below
json = "{}"
# create an instance of AppMediaVideoState from a JSON string
app_media_video_state_instance = AppMediaVideoState.from_json(json)
# print the JSON string representation of the object
print(AppMediaVideoState.to_json())

# convert the object into a dict
app_media_video_state_dict = app_media_video_state_instance.to_dict()
# create an instance of AppMediaVideoState from a dict
app_media_video_state_from_dict = AppMediaVideoState.from_dict(app_media_video_state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



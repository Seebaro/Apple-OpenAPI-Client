# AppClipsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppClip]**](AppClip.md) |  | 
**included** | [**List[AppClipsResponseIncludedInner]**](AppClipsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_clips_response import AppClipsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipsResponse from a JSON string
app_clips_response_instance = AppClipsResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipsResponse.to_json())

# convert the object into a dict
app_clips_response_dict = app_clips_response_instance.to_dict()
# create an instance of AppClipsResponse from a dict
app_clips_response_from_dict = AppClipsResponse.from_dict(app_clips_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



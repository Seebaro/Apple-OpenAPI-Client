# AppClipHeaderImageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipHeaderImageUpdateRequestData**](AppClipHeaderImageUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_clip_header_image_update_request import AppClipHeaderImageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipHeaderImageUpdateRequest from a JSON string
app_clip_header_image_update_request_instance = AppClipHeaderImageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppClipHeaderImageUpdateRequest.to_json())

# convert the object into a dict
app_clip_header_image_update_request_dict = app_clip_header_image_update_request_instance.to_dict()
# create an instance of AppClipHeaderImageUpdateRequest from a dict
app_clip_header_image_update_request_from_dict = AppClipHeaderImageUpdateRequest.from_dict(app_clip_header_image_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



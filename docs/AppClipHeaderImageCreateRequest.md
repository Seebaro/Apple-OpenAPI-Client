# AppClipHeaderImageCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipHeaderImageCreateRequestData**](AppClipHeaderImageCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_clip_header_image_create_request import AppClipHeaderImageCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipHeaderImageCreateRequest from a JSON string
app_clip_header_image_create_request_instance = AppClipHeaderImageCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppClipHeaderImageCreateRequest.to_json())

# convert the object into a dict
app_clip_header_image_create_request_dict = app_clip_header_image_create_request_instance.to_dict()
# create an instance of AppClipHeaderImageCreateRequest from a dict
app_clip_header_image_create_request_from_dict = AppClipHeaderImageCreateRequest.from_dict(app_clip_header_image_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



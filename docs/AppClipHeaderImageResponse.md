# AppClipHeaderImageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppClipHeaderImage**](AppClipHeaderImage.md) |  | 
**included** | [**List[AppClipDefaultExperienceLocalization]**](AppClipDefaultExperienceLocalization.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_clip_header_image_response import AppClipHeaderImageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppClipHeaderImageResponse from a JSON string
app_clip_header_image_response_instance = AppClipHeaderImageResponse.from_json(json)
# print the JSON string representation of the object
print(AppClipHeaderImageResponse.to_json())

# convert the object into a dict
app_clip_header_image_response_dict = app_clip_header_image_response_instance.to_dict()
# create an instance of AppClipHeaderImageResponse from a dict
app_clip_header_image_response_from_dict = AppClipHeaderImageResponse.from_dict(app_clip_header_image_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



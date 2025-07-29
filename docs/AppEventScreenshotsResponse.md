# AppEventScreenshotsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEventScreenshot]**](AppEventScreenshot.md) |  | 
**included** | [**List[AppEventLocalization]**](AppEventLocalization.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_screenshots_response import AppEventScreenshotsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshotsResponse from a JSON string
app_event_screenshots_response_instance = AppEventScreenshotsResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshotsResponse.to_json())

# convert the object into a dict
app_event_screenshots_response_dict = app_event_screenshots_response_instance.to_dict()
# create an instance of AppEventScreenshotsResponse from a dict
app_event_screenshots_response_from_dict = AppEventScreenshotsResponse.from_dict(app_event_screenshots_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



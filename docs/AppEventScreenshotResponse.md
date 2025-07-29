# AppEventScreenshotResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventScreenshot**](AppEventScreenshot.md) |  | 
**included** | [**List[AppEventLocalization]**](AppEventLocalization.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_event_screenshot_response import AppEventScreenshotResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshotResponse from a JSON string
app_event_screenshot_response_instance = AppEventScreenshotResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshotResponse.to_json())

# convert the object into a dict
app_event_screenshot_response_dict = app_event_screenshot_response_instance.to_dict()
# create an instance of AppEventScreenshotResponse from a dict
app_event_screenshot_response_from_dict = AppEventScreenshotResponse.from_dict(app_event_screenshot_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



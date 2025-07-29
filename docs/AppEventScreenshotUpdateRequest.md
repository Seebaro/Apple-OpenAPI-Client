# AppEventScreenshotUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventScreenshotUpdateRequestData**](AppEventScreenshotUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_event_screenshot_update_request import AppEventScreenshotUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshotUpdateRequest from a JSON string
app_event_screenshot_update_request_instance = AppEventScreenshotUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshotUpdateRequest.to_json())

# convert the object into a dict
app_event_screenshot_update_request_dict = app_event_screenshot_update_request_instance.to_dict()
# create an instance of AppEventScreenshotUpdateRequest from a dict
app_event_screenshot_update_request_from_dict = AppEventScreenshotUpdateRequest.from_dict(app_event_screenshot_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



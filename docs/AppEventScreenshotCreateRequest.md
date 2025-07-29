# AppEventScreenshotCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventScreenshotCreateRequestData**](AppEventScreenshotCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_event_screenshot_create_request import AppEventScreenshotCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshotCreateRequest from a JSON string
app_event_screenshot_create_request_instance = AppEventScreenshotCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshotCreateRequest.to_json())

# convert the object into a dict
app_event_screenshot_create_request_dict = app_event_screenshot_create_request_instance.to_dict()
# create an instance of AppEventScreenshotCreateRequest from a dict
app_event_screenshot_create_request_from_dict = AppEventScreenshotCreateRequest.from_dict(app_event_screenshot_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



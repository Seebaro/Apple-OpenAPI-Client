# AppEventScreenshotUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventScreenshotUpdateRequestDataAttributes**](AppEventScreenshotUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_screenshot_update_request_data import AppEventScreenshotUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshotUpdateRequestData from a JSON string
app_event_screenshot_update_request_data_instance = AppEventScreenshotUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshotUpdateRequestData.to_json())

# convert the object into a dict
app_event_screenshot_update_request_data_dict = app_event_screenshot_update_request_data_instance.to_dict()
# create an instance of AppEventScreenshotUpdateRequestData from a dict
app_event_screenshot_update_request_data_from_dict = AppEventScreenshotUpdateRequestData.from_dict(app_event_screenshot_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AppEventScreenshot


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventScreenshotAttributes**](AppEventScreenshotAttributes.md) |  | [optional] 
**relationships** | [**AppEventScreenshotRelationships**](AppEventScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_screenshot import AppEventScreenshot

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventScreenshot from a JSON string
app_event_screenshot_instance = AppEventScreenshot.from_json(json)
# print the JSON string representation of the object
print(AppEventScreenshot.to_json())

# convert the object into a dict
app_event_screenshot_dict = app_event_screenshot_instance.to_dict()
# create an instance of AppEventScreenshot from a dict
app_event_screenshot_from_dict = AppEventScreenshot.from_dict(app_event_screenshot_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



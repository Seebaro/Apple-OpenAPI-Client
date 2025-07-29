# AppScreenshot


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppScreenshotAttributes**](AppScreenshotAttributes.md) |  | [optional] 
**relationships** | [**AppScreenshotRelationships**](AppScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_screenshot import AppScreenshot

# TODO update the JSON string below
json = "{}"
# create an instance of AppScreenshot from a JSON string
app_screenshot_instance = AppScreenshot.from_json(json)
# print the JSON string representation of the object
print(AppScreenshot.to_json())

# convert the object into a dict
app_screenshot_dict = app_screenshot_instance.to_dict()
# create an instance of AppScreenshot from a dict
app_screenshot_from_dict = AppScreenshot.from_dict(app_screenshot_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



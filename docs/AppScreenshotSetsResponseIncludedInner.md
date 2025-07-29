# AppScreenshotSetsResponseIncludedInner


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
from openapi_client.models.app_screenshot_sets_response_included_inner import AppScreenshotSetsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppScreenshotSetsResponseIncludedInner from a JSON string
app_screenshot_sets_response_included_inner_instance = AppScreenshotSetsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppScreenshotSetsResponseIncludedInner.to_json())

# convert the object into a dict
app_screenshot_sets_response_included_inner_dict = app_screenshot_sets_response_included_inner_instance.to_dict()
# create an instance of AppScreenshotSetsResponseIncludedInner from a dict
app_screenshot_sets_response_included_inner_from_dict = AppScreenshotSetsResponseIncludedInner.from_dict(app_screenshot_sets_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



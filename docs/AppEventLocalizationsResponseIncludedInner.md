# AppEventLocalizationsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventVideoClipAttributes**](AppEventVideoClipAttributes.md) |  | [optional] 
**relationships** | [**AppEventScreenshotRelationships**](AppEventScreenshotRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localizations_response_included_inner import AppEventLocalizationsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationsResponseIncludedInner from a JSON string
app_event_localizations_response_included_inner_instance = AppEventLocalizationsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationsResponseIncludedInner.to_json())

# convert the object into a dict
app_event_localizations_response_included_inner_dict = app_event_localizations_response_included_inner_instance.to_dict()
# create an instance of AppEventLocalizationsResponseIncludedInner from a dict
app_event_localizations_response_included_inner_from_dict = AppEventLocalizationsResponseIncludedInner.from_dict(app_event_localizations_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



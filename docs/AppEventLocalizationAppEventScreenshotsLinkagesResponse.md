# AppEventLocalizationAppEventScreenshotsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEventLocalizationRelationshipsAppEventScreenshotsDataInner]**](AppEventLocalizationRelationshipsAppEventScreenshotsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localization_app_event_screenshots_linkages_response import AppEventLocalizationAppEventScreenshotsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationAppEventScreenshotsLinkagesResponse from a JSON string
app_event_localization_app_event_screenshots_linkages_response_instance = AppEventLocalizationAppEventScreenshotsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationAppEventScreenshotsLinkagesResponse.to_json())

# convert the object into a dict
app_event_localization_app_event_screenshots_linkages_response_dict = app_event_localization_app_event_screenshots_linkages_response_instance.to_dict()
# create an instance of AppEventLocalizationAppEventScreenshotsLinkagesResponse from a dict
app_event_localization_app_event_screenshots_linkages_response_from_dict = AppEventLocalizationAppEventScreenshotsLinkagesResponse.from_dict(app_event_localization_app_event_screenshots_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



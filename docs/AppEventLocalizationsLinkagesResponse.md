# AppEventLocalizationsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEventScreenshotRelationshipsAppEventLocalizationData]**](AppEventScreenshotRelationshipsAppEventLocalizationData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localizations_linkages_response import AppEventLocalizationsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationsLinkagesResponse from a JSON string
app_event_localizations_linkages_response_instance = AppEventLocalizationsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationsLinkagesResponse.to_json())

# convert the object into a dict
app_event_localizations_linkages_response_dict = app_event_localizations_linkages_response_instance.to_dict()
# create an instance of AppEventLocalizationsLinkagesResponse from a dict
app_event_localizations_linkages_response_from_dict = AppEventLocalizationsLinkagesResponse.from_dict(app_event_localizations_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



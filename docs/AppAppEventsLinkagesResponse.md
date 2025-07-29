# AppAppEventsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEventLocalizationRelationshipsAppEventData]**](AppEventLocalizationRelationshipsAppEventData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_app_events_linkages_response import AppAppEventsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppEventsLinkagesResponse from a JSON string
app_app_events_linkages_response_instance = AppAppEventsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppEventsLinkagesResponse.to_json())

# convert the object into a dict
app_app_events_linkages_response_dict = app_app_events_linkages_response_instance.to_dict()
# create an instance of AppAppEventsLinkagesResponse from a dict
app_app_events_linkages_response_from_dict = AppAppEventsLinkagesResponse.from_dict(app_app_events_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



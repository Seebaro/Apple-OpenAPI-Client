# AppEventsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEvent]**](AppEvent.md) |  | 
**included** | [**List[AppEventLocalization]**](AppEventLocalization.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_events_response import AppEventsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventsResponse from a JSON string
app_events_response_instance = AppEventsResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventsResponse.to_json())

# convert the object into a dict
app_events_response_dict = app_events_response_instance.to_dict()
# create an instance of AppEventsResponse from a dict
app_events_response_from_dict = AppEventsResponse.from_dict(app_events_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AppEventLocalizationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppEventLocalization]**](AppEventLocalization.md) |  | 
**included** | [**List[AppEventLocalizationsResponseIncludedInner]**](AppEventLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localizations_response import AppEventLocalizationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationsResponse from a JSON string
app_event_localizations_response_instance = AppEventLocalizationsResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationsResponse.to_json())

# convert the object into a dict
app_event_localizations_response_dict = app_event_localizations_response_instance.to_dict()
# create an instance of AppEventLocalizationsResponse from a dict
app_event_localizations_response_from_dict = AppEventLocalizationsResponse.from_dict(app_event_localizations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



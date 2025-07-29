# AppEventLocalizationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventLocalization**](AppEventLocalization.md) |  | 
**included** | [**List[AppEventLocalizationsResponseIncludedInner]**](AppEventLocalizationsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_event_localization_response import AppEventLocalizationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationResponse from a JSON string
app_event_localization_response_instance = AppEventLocalizationResponse.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationResponse.to_json())

# convert the object into a dict
app_event_localization_response_dict = app_event_localization_response_instance.to_dict()
# create an instance of AppEventLocalizationResponse from a dict
app_event_localization_response_from_dict = AppEventLocalizationResponse.from_dict(app_event_localization_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



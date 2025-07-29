# AppEventLocalizationUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventLocalizationUpdateRequestData**](AppEventLocalizationUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_event_localization_update_request import AppEventLocalizationUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationUpdateRequest from a JSON string
app_event_localization_update_request_instance = AppEventLocalizationUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationUpdateRequest.to_json())

# convert the object into a dict
app_event_localization_update_request_dict = app_event_localization_update_request_instance.to_dict()
# create an instance of AppEventLocalizationUpdateRequest from a dict
app_event_localization_update_request_from_dict = AppEventLocalizationUpdateRequest.from_dict(app_event_localization_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AppEventLocalizationCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventLocalizationCreateRequestData**](AppEventLocalizationCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_event_localization_create_request import AppEventLocalizationCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationCreateRequest from a JSON string
app_event_localization_create_request_instance = AppEventLocalizationCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationCreateRequest.to_json())

# convert the object into a dict
app_event_localization_create_request_dict = app_event_localization_create_request_instance.to_dict()
# create an instance of AppEventLocalizationCreateRequest from a dict
app_event_localization_create_request_from_dict = AppEventLocalizationCreateRequest.from_dict(app_event_localization_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AppEventLocalizationCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppEventLocalizationCreateRequestDataAttributes**](AppEventLocalizationCreateRequestDataAttributes.md) |  | 
**relationships** | [**AppEventLocalizationCreateRequestDataRelationships**](AppEventLocalizationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_event_localization_create_request_data import AppEventLocalizationCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationCreateRequestData from a JSON string
app_event_localization_create_request_data_instance = AppEventLocalizationCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationCreateRequestData.to_json())

# convert the object into a dict
app_event_localization_create_request_data_dict = app_event_localization_create_request_data_instance.to_dict()
# create an instance of AppEventLocalizationCreateRequestData from a dict
app_event_localization_create_request_data_from_dict = AppEventLocalizationCreateRequestData.from_dict(app_event_localization_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AppEventLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventLocalizationAttributes**](AppEventLocalizationAttributes.md) |  | [optional] 
**relationships** | [**AppEventLocalizationRelationships**](AppEventLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localization import AppEventLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalization from a JSON string
app_event_localization_instance = AppEventLocalization.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalization.to_json())

# convert the object into a dict
app_event_localization_dict = app_event_localization_instance.to_dict()
# create an instance of AppEventLocalization from a dict
app_event_localization_from_dict = AppEventLocalization.from_dict(app_event_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AppEventLocalizationAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**locale** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**short_description** | **str** |  | [optional] 
**long_description** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.app_event_localization_attributes import AppEventLocalizationAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventLocalizationAttributes from a JSON string
app_event_localization_attributes_instance = AppEventLocalizationAttributes.from_json(json)
# print the JSON string representation of the object
print(AppEventLocalizationAttributes.to_json())

# convert the object into a dict
app_event_localization_attributes_dict = app_event_localization_attributes_instance.to_dict()
# create an instance of AppEventLocalizationAttributes from a dict
app_event_localization_attributes_from_dict = AppEventLocalizationAttributes.from_dict(app_event_localization_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



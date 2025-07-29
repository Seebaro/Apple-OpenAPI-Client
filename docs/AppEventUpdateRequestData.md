# AppEventUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventUpdateRequestDataAttributes**](AppEventUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_event_update_request_data import AppEventUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventUpdateRequestData from a JSON string
app_event_update_request_data_instance = AppEventUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppEventUpdateRequestData.to_json())

# convert the object into a dict
app_event_update_request_data_dict = app_event_update_request_data_instance.to_dict()
# create an instance of AppEventUpdateRequestData from a dict
app_event_update_request_data_from_dict = AppEventUpdateRequestData.from_dict(app_event_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



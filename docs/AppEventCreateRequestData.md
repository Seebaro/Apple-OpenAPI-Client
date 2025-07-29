# AppEventCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppEventCreateRequestDataAttributes**](AppEventCreateRequestDataAttributes.md) |  | 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_event_create_request_data import AppEventCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventCreateRequestData from a JSON string
app_event_create_request_data_instance = AppEventCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppEventCreateRequestData.to_json())

# convert the object into a dict
app_event_create_request_data_dict = app_event_create_request_data_instance.to_dict()
# create an instance of AppEventCreateRequestData from a dict
app_event_create_request_data_from_dict = AppEventCreateRequestData.from_dict(app_event_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



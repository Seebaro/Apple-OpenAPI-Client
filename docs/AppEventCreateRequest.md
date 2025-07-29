# AppEventCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppEventCreateRequestData**](AppEventCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.app_event_create_request import AppEventCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppEventCreateRequest from a JSON string
app_event_create_request_instance = AppEventCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppEventCreateRequest.to_json())

# convert the object into a dict
app_event_create_request_dict = app_event_create_request_instance.to_dict()
# create an instance of AppEventCreateRequest from a dict
app_event_create_request_from_dict = AppEventCreateRequest.from_dict(app_event_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



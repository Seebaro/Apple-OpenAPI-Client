# AppAvailabilityV2CreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppAvailabilityV2CreateRequestData**](AppAvailabilityV2CreateRequestData.md) |  | 
**included** | [**List[TerritoryAvailabilityInlineCreate]**](TerritoryAvailabilityInlineCreate.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_availability_v2_create_request import AppAvailabilityV2CreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2CreateRequest from a JSON string
app_availability_v2_create_request_instance = AppAvailabilityV2CreateRequest.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2CreateRequest.to_json())

# convert the object into a dict
app_availability_v2_create_request_dict = app_availability_v2_create_request_instance.to_dict()
# create an instance of AppAvailabilityV2CreateRequest from a dict
app_availability_v2_create_request_from_dict = AppAvailabilityV2CreateRequest.from_dict(app_availability_v2_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



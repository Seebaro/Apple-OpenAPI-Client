# AppAvailabilityV2CreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AppAvailabilityV2CreateRequestDataAttributes**](AppAvailabilityV2CreateRequestDataAttributes.md) |  | 
**relationships** | [**AppAvailabilityV2CreateRequestDataRelationships**](AppAvailabilityV2CreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.app_availability_v2_create_request_data import AppAvailabilityV2CreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2CreateRequestData from a JSON string
app_availability_v2_create_request_data_instance = AppAvailabilityV2CreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2CreateRequestData.to_json())

# convert the object into a dict
app_availability_v2_create_request_data_dict = app_availability_v2_create_request_data_instance.to_dict()
# create an instance of AppAvailabilityV2CreateRequestData from a dict
app_availability_v2_create_request_data_from_dict = AppAvailabilityV2CreateRequestData.from_dict(app_availability_v2_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



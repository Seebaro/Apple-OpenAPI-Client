# AppAvailabilityV2Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppAvailabilityV2**](AppAvailabilityV2.md) |  | 
**included** | [**List[TerritoryAvailability]**](TerritoryAvailability.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_availability_v2_response import AppAvailabilityV2Response

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2Response from a JSON string
app_availability_v2_response_instance = AppAvailabilityV2Response.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2Response.to_json())

# convert the object into a dict
app_availability_v2_response_dict = app_availability_v2_response_instance.to_dict()
# create an instance of AppAvailabilityV2Response from a dict
app_availability_v2_response_from_dict = AppAvailabilityV2Response.from_dict(app_availability_v2_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



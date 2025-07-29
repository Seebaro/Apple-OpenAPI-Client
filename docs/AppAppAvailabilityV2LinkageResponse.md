# AppAppAvailabilityV2LinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppAppAvailabilityV2LinkageResponseData**](AppAppAvailabilityV2LinkageResponseData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_app_availability_v2_linkage_response import AppAppAvailabilityV2LinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppAppAvailabilityV2LinkageResponse from a JSON string
app_app_availability_v2_linkage_response_instance = AppAppAvailabilityV2LinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppAppAvailabilityV2LinkageResponse.to_json())

# convert the object into a dict
app_app_availability_v2_linkage_response_dict = app_app_availability_v2_linkage_response_instance.to_dict()
# create an instance of AppAppAvailabilityV2LinkageResponse from a dict
app_app_availability_v2_linkage_response_from_dict = AppAppAvailabilityV2LinkageResponse.from_dict(app_app_availability_v2_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



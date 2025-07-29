# AppAvailabilityV2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppAvailabilityV2Attributes**](AppAvailabilityV2Attributes.md) |  | [optional] 
**relationships** | [**AppAvailabilityV2Relationships**](AppAvailabilityV2Relationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_availability_v2 import AppAvailabilityV2

# TODO update the JSON string below
json = "{}"
# create an instance of AppAvailabilityV2 from a JSON string
app_availability_v2_instance = AppAvailabilityV2.from_json(json)
# print the JSON string representation of the object
print(AppAvailabilityV2.to_json())

# convert the object into a dict
app_availability_v2_dict = app_availability_v2_instance.to_dict()
# create an instance of AppAvailabilityV2 from a dict
app_availability_v2_from_dict = AppAvailabilityV2.from_dict(app_availability_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



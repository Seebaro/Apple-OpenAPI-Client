# CiTestDestination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_type_name** | **str** |  | [optional] 
**device_type_identifier** | **str** |  | [optional] 
**runtime_name** | **str** |  | [optional] 
**runtime_identifier** | **str** |  | [optional] 
**kind** | [**CiTestDestinationKind**](CiTestDestinationKind.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_test_destination import CiTestDestination

# TODO update the JSON string below
json = "{}"
# create an instance of CiTestDestination from a JSON string
ci_test_destination_instance = CiTestDestination.from_json(json)
# print the JSON string representation of the object
print(CiTestDestination.to_json())

# convert the object into a dict
ci_test_destination_dict = ci_test_destination_instance.to_dict()
# create an instance of CiTestDestination from a dict
ci_test_destination_from_dict = CiTestDestination.from_dict(ci_test_destination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



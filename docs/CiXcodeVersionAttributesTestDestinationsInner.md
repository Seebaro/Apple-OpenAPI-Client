# CiXcodeVersionAttributesTestDestinationsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**device_type_name** | **str** |  | [optional] 
**device_type_identifier** | **str** |  | [optional] 
**available_runtimes** | [**List[CiXcodeVersionAttributesTestDestinationsInnerAvailableRuntimesInner]**](CiXcodeVersionAttributesTestDestinationsInnerAvailableRuntimesInner.md) |  | [optional] 
**kind** | [**CiTestDestinationKind**](CiTestDestinationKind.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_xcode_version_attributes_test_destinations_inner import CiXcodeVersionAttributesTestDestinationsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CiXcodeVersionAttributesTestDestinationsInner from a JSON string
ci_xcode_version_attributes_test_destinations_inner_instance = CiXcodeVersionAttributesTestDestinationsInner.from_json(json)
# print the JSON string representation of the object
print(CiXcodeVersionAttributesTestDestinationsInner.to_json())

# convert the object into a dict
ci_xcode_version_attributes_test_destinations_inner_dict = ci_xcode_version_attributes_test_destinations_inner_instance.to_dict()
# create an instance of CiXcodeVersionAttributesTestDestinationsInner from a dict
ci_xcode_version_attributes_test_destinations_inner_from_dict = CiXcodeVersionAttributesTestDestinationsInner.from_dict(ci_xcode_version_attributes_test_destinations_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



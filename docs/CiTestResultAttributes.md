# CiTestResultAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**class_name** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**status** | [**CiTestStatus**](CiTestStatus.md) |  | [optional] 
**file_source** | [**FileLocation**](FileLocation.md) |  | [optional] 
**message** | **str** |  | [optional] 
**destination_test_results** | [**List[CiTestResultAttributesDestinationTestResultsInner]**](CiTestResultAttributesDestinationTestResultsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_test_result_attributes import CiTestResultAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiTestResultAttributes from a JSON string
ci_test_result_attributes_instance = CiTestResultAttributes.from_json(json)
# print the JSON string representation of the object
print(CiTestResultAttributes.to_json())

# convert the object into a dict
ci_test_result_attributes_dict = ci_test_result_attributes_instance.to_dict()
# create an instance of CiTestResultAttributes from a dict
ci_test_result_attributes_from_dict = CiTestResultAttributes.from_dict(ci_test_result_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



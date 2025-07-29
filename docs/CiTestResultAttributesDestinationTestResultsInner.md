# CiTestResultAttributesDestinationTestResultsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**uuid** | **str** |  | [optional] 
**device_name** | **str** |  | [optional] 
**os_version** | **str** |  | [optional] 
**status** | [**CiTestStatus**](CiTestStatus.md) |  | [optional] 
**duration** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.ci_test_result_attributes_destination_test_results_inner import CiTestResultAttributesDestinationTestResultsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CiTestResultAttributesDestinationTestResultsInner from a JSON string
ci_test_result_attributes_destination_test_results_inner_instance = CiTestResultAttributesDestinationTestResultsInner.from_json(json)
# print the JSON string representation of the object
print(CiTestResultAttributesDestinationTestResultsInner.to_json())

# convert the object into a dict
ci_test_result_attributes_destination_test_results_inner_dict = ci_test_result_attributes_destination_test_results_inner_instance.to_dict()
# create an instance of CiTestResultAttributesDestinationTestResultsInner from a dict
ci_test_result_attributes_destination_test_results_inner_from_dict = CiTestResultAttributesDestinationTestResultsInner.from_dict(ci_test_result_attributes_destination_test_results_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



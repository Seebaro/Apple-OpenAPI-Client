# CiTestResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiTestResultAttributes**](CiTestResultAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_test_result import CiTestResult

# TODO update the JSON string below
json = "{}"
# create an instance of CiTestResult from a JSON string
ci_test_result_instance = CiTestResult.from_json(json)
# print the JSON string representation of the object
print(CiTestResult.to_json())

# convert the object into a dict
ci_test_result_dict = ci_test_result_instance.to_dict()
# create an instance of CiTestResult from a dict
ci_test_result_from_dict = CiTestResult.from_dict(ci_test_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



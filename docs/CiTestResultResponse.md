# CiTestResultResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiTestResult**](CiTestResult.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_test_result_response import CiTestResultResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiTestResultResponse from a JSON string
ci_test_result_response_instance = CiTestResultResponse.from_json(json)
# print the JSON string representation of the object
print(CiTestResultResponse.to_json())

# convert the object into a dict
ci_test_result_response_dict = ci_test_result_response_instance.to_dict()
# create an instance of CiTestResultResponse from a dict
ci_test_result_response_from_dict = CiTestResultResponse.from_dict(ci_test_result_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



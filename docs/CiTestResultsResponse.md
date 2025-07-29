# CiTestResultsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiTestResult]**](CiTestResult.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_test_results_response import CiTestResultsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiTestResultsResponse from a JSON string
ci_test_results_response_instance = CiTestResultsResponse.from_json(json)
# print the JSON string representation of the object
print(CiTestResultsResponse.to_json())

# convert the object into a dict
ci_test_results_response_dict = ci_test_results_response_instance.to_dict()
# create an instance of CiTestResultsResponse from a dict
ci_test_results_response_from_dict = CiTestResultsResponse.from_dict(ci_test_results_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



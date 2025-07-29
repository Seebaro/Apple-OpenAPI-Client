# CiBuildRunsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiBuildRun]**](CiBuildRun.md) |  | 
**included** | [**List[CiBuildRunsResponseIncludedInner]**](CiBuildRunsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_runs_response import CiBuildRunsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunsResponse from a JSON string
ci_build_runs_response_instance = CiBuildRunsResponse.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunsResponse.to_json())

# convert the object into a dict
ci_build_runs_response_dict = ci_build_runs_response_instance.to_dict()
# create an instance of CiBuildRunsResponse from a dict
ci_build_runs_response_from_dict = CiBuildRunsResponse.from_dict(ci_build_runs_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



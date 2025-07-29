# CiBuildRunResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiBuildRun**](CiBuildRun.md) |  | 
**included** | [**List[CiBuildRunsResponseIncludedInner]**](CiBuildRunsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_build_run_response import CiBuildRunResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunResponse from a JSON string
ci_build_run_response_instance = CiBuildRunResponse.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunResponse.to_json())

# convert the object into a dict
ci_build_run_response_dict = ci_build_run_response_instance.to_dict()
# create an instance of CiBuildRunResponse from a dict
ci_build_run_response_from_dict = CiBuildRunResponse.from_dict(ci_build_run_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



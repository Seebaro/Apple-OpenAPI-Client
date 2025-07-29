# CiBuildRunCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiBuildRunCreateRequestData**](CiBuildRunCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.ci_build_run_create_request import CiBuildRunCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunCreateRequest from a JSON string
ci_build_run_create_request_instance = CiBuildRunCreateRequest.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunCreateRequest.to_json())

# convert the object into a dict
ci_build_run_create_request_dict = ci_build_run_create_request_instance.to_dict()
# create an instance of CiBuildRunCreateRequest from a dict
ci_build_run_create_request_from_dict = CiBuildRunCreateRequest.from_dict(ci_build_run_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiBuildActionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiBuildAction**](CiBuildAction.md) |  | 
**included** | [**List[CiBuildRun]**](CiBuildRun.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_build_action_response import CiBuildActionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildActionResponse from a JSON string
ci_build_action_response_instance = CiBuildActionResponse.from_json(json)
# print the JSON string representation of the object
print(CiBuildActionResponse.to_json())

# convert the object into a dict
ci_build_action_response_dict = ci_build_action_response_instance.to_dict()
# create an instance of CiBuildActionResponse from a dict
ci_build_action_response_from_dict = CiBuildActionResponse.from_dict(ci_build_action_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiBuildActionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiBuildAction]**](CiBuildAction.md) |  | 
**included** | [**List[CiBuildRun]**](CiBuildRun.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_actions_response import CiBuildActionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildActionsResponse from a JSON string
ci_build_actions_response_instance = CiBuildActionsResponse.from_json(json)
# print the JSON string representation of the object
print(CiBuildActionsResponse.to_json())

# convert the object into a dict
ci_build_actions_response_dict = ci_build_actions_response_instance.to_dict()
# create an instance of CiBuildActionsResponse from a dict
ci_build_actions_response_from_dict = CiBuildActionsResponse.from_dict(ci_build_actions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



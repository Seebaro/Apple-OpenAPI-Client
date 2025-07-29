# CiBuildActionBuildRunLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiBuildActionRelationshipsBuildRunData**](CiBuildActionRelationshipsBuildRunData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_build_action_build_run_linkage_response import CiBuildActionBuildRunLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildActionBuildRunLinkageResponse from a JSON string
ci_build_action_build_run_linkage_response_instance = CiBuildActionBuildRunLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(CiBuildActionBuildRunLinkageResponse.to_json())

# convert the object into a dict
ci_build_action_build_run_linkage_response_dict = ci_build_action_build_run_linkage_response_instance.to_dict()
# create an instance of CiBuildActionBuildRunLinkageResponse from a dict
ci_build_action_build_run_linkage_response_from_dict = CiBuildActionBuildRunLinkageResponse.from_dict(ci_build_action_build_run_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



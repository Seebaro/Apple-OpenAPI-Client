# CiWorkflowBuildRunsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiBuildActionRelationshipsBuildRunData]**](CiBuildActionRelationshipsBuildRunData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflow_build_runs_linkages_response import CiWorkflowBuildRunsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowBuildRunsLinkagesResponse from a JSON string
ci_workflow_build_runs_linkages_response_instance = CiWorkflowBuildRunsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowBuildRunsLinkagesResponse.to_json())

# convert the object into a dict
ci_workflow_build_runs_linkages_response_dict = ci_workflow_build_runs_linkages_response_instance.to_dict()
# create an instance of CiWorkflowBuildRunsLinkagesResponse from a dict
ci_workflow_build_runs_linkages_response_from_dict = CiWorkflowBuildRunsLinkagesResponse.from_dict(ci_workflow_build_runs_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



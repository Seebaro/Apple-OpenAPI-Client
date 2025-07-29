# CiWorkflowRepositoryLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiProductRelationshipsPrimaryRepositoriesDataInner**](CiProductRelationshipsPrimaryRepositoriesDataInner.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_workflow_repository_linkage_response import CiWorkflowRepositoryLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowRepositoryLinkageResponse from a JSON string
ci_workflow_repository_linkage_response_instance = CiWorkflowRepositoryLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowRepositoryLinkageResponse.to_json())

# convert the object into a dict
ci_workflow_repository_linkage_response_dict = ci_workflow_repository_linkage_response_instance.to_dict()
# create an instance of CiWorkflowRepositoryLinkageResponse from a dict
ci_workflow_repository_linkage_response_from_dict = CiWorkflowRepositoryLinkageResponse.from_dict(ci_workflow_repository_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



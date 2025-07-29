# CiWorkflowRelationshipsRepository


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**CiProductRelationshipsPrimaryRepositoriesDataInner**](CiProductRelationshipsPrimaryRepositoriesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflow_relationships_repository import CiWorkflowRelationshipsRepository

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowRelationshipsRepository from a JSON string
ci_workflow_relationships_repository_instance = CiWorkflowRelationshipsRepository.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowRelationshipsRepository.to_json())

# convert the object into a dict
ci_workflow_relationships_repository_dict = ci_workflow_relationships_repository_instance.to_dict()
# create an instance of CiWorkflowRelationshipsRepository from a dict
ci_workflow_relationships_repository_from_dict = CiWorkflowRelationshipsRepository.from_dict(ci_workflow_relationships_repository_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



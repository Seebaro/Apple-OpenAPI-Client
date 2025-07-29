# CiBuildRunCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**build_run** | [**CiBuildRunCreateRequestDataRelationshipsBuildRun**](CiBuildRunCreateRequestDataRelationshipsBuildRun.md) |  | [optional] 
**workflow** | [**CiBuildRunRelationshipsWorkflow**](CiBuildRunRelationshipsWorkflow.md) |  | [optional] 
**source_branch_or_tag** | [**CiBuildRunRelationshipsSourceBranchOrTag**](CiBuildRunRelationshipsSourceBranchOrTag.md) |  | [optional] 
**pull_request** | [**CiBuildRunRelationshipsPullRequest**](CiBuildRunRelationshipsPullRequest.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_run_create_request_data_relationships import CiBuildRunCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunCreateRequestDataRelationships from a JSON string
ci_build_run_create_request_data_relationships_instance = CiBuildRunCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunCreateRequestDataRelationships.to_json())

# convert the object into a dict
ci_build_run_create_request_data_relationships_dict = ci_build_run_create_request_data_relationships_instance.to_dict()
# create an instance of CiBuildRunCreateRequestDataRelationships from a dict
ci_build_run_create_request_data_relationships_from_dict = CiBuildRunCreateRequestDataRelationships.from_dict(ci_build_run_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



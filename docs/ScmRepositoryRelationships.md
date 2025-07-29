# ScmRepositoryRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**scm_provider** | [**ScmRepositoryRelationshipsScmProvider**](ScmRepositoryRelationshipsScmProvider.md) |  | [optional] 
**default_branch** | [**CiBuildRunRelationshipsSourceBranchOrTag**](CiBuildRunRelationshipsSourceBranchOrTag.md) |  | [optional] 
**git_references** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**pull_requests** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_repository_relationships import ScmRepositoryRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepositoryRelationships from a JSON string
scm_repository_relationships_instance = ScmRepositoryRelationships.from_json(json)
# print the JSON string representation of the object
print(ScmRepositoryRelationships.to_json())

# convert the object into a dict
scm_repository_relationships_dict = scm_repository_relationships_instance.to_dict()
# create an instance of ScmRepositoryRelationships from a dict
scm_repository_relationships_from_dict = ScmRepositoryRelationships.from_dict(scm_repository_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



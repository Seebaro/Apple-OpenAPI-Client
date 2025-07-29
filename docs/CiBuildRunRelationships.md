# CiBuildRunRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**builds** | [**AppRelationshipsBuilds**](AppRelationshipsBuilds.md) |  | [optional] 
**workflow** | [**CiBuildRunRelationshipsWorkflow**](CiBuildRunRelationshipsWorkflow.md) |  | [optional] 
**product** | [**CiBuildRunRelationshipsProduct**](CiBuildRunRelationshipsProduct.md) |  | [optional] 
**source_branch_or_tag** | [**CiBuildRunRelationshipsSourceBranchOrTag**](CiBuildRunRelationshipsSourceBranchOrTag.md) |  | [optional] 
**destination_branch** | [**CiBuildRunRelationshipsSourceBranchOrTag**](CiBuildRunRelationshipsSourceBranchOrTag.md) |  | [optional] 
**actions** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**pull_request** | [**CiBuildRunRelationshipsPullRequest**](CiBuildRunRelationshipsPullRequest.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_run_relationships import CiBuildRunRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunRelationships from a JSON string
ci_build_run_relationships_instance = CiBuildRunRelationships.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunRelationships.to_json())

# convert the object into a dict
ci_build_run_relationships_dict = ci_build_run_relationships_instance.to_dict()
# create an instance of CiBuildRunRelationships from a dict
ci_build_run_relationships_from_dict = CiBuildRunRelationships.from_dict(ci_build_run_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



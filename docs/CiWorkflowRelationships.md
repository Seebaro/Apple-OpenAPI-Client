# CiWorkflowRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product** | [**CiBuildRunRelationshipsProduct**](CiBuildRunRelationshipsProduct.md) |  | [optional] 
**repository** | [**CiWorkflowRelationshipsRepository**](CiWorkflowRelationshipsRepository.md) |  | [optional] 
**xcode_version** | [**CiWorkflowRelationshipsXcodeVersion**](CiWorkflowRelationshipsXcodeVersion.md) |  | [optional] 
**mac_os_version** | [**CiWorkflowRelationshipsMacOsVersion**](CiWorkflowRelationshipsMacOsVersion.md) |  | [optional] 
**build_runs** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflow_relationships import CiWorkflowRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowRelationships from a JSON string
ci_workflow_relationships_instance = CiWorkflowRelationships.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowRelationships.to_json())

# convert the object into a dict
ci_workflow_relationships_dict = ci_workflow_relationships_instance.to_dict()
# create an instance of CiWorkflowRelationships from a dict
ci_workflow_relationships_from_dict = CiWorkflowRelationships.from_dict(ci_workflow_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



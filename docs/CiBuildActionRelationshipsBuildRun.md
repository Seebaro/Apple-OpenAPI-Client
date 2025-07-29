# CiBuildActionRelationshipsBuildRun


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**CiBuildActionRelationshipsBuildRunData**](CiBuildActionRelationshipsBuildRunData.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_action_relationships_build_run import CiBuildActionRelationshipsBuildRun

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildActionRelationshipsBuildRun from a JSON string
ci_build_action_relationships_build_run_instance = CiBuildActionRelationshipsBuildRun.from_json(json)
# print the JSON string representation of the object
print(CiBuildActionRelationshipsBuildRun.to_json())

# convert the object into a dict
ci_build_action_relationships_build_run_dict = ci_build_action_relationships_build_run_instance.to_dict()
# create an instance of CiBuildActionRelationshipsBuildRun from a dict
ci_build_action_relationships_build_run_from_dict = CiBuildActionRelationshipsBuildRun.from_dict(ci_build_action_relationships_build_run_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



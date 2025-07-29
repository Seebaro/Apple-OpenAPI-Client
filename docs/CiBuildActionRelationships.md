# CiBuildActionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**build_run** | [**CiBuildActionRelationshipsBuildRun**](CiBuildActionRelationshipsBuildRun.md) |  | [optional] 
**artifacts** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**issues** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**test_results** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_action_relationships import CiBuildActionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildActionRelationships from a JSON string
ci_build_action_relationships_instance = CiBuildActionRelationships.from_json(json)
# print the JSON string representation of the object
print(CiBuildActionRelationships.to_json())

# convert the object into a dict
ci_build_action_relationships_dict = ci_build_action_relationships_instance.to_dict()
# create an instance of CiBuildActionRelationships from a dict
ci_build_action_relationships_from_dict = CiBuildActionRelationships.from_dict(ci_build_action_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



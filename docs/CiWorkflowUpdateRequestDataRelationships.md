# CiWorkflowUpdateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**xcode_version** | [**CiWorkflowRelationshipsXcodeVersion**](CiWorkflowRelationshipsXcodeVersion.md) |  | [optional] 
**mac_os_version** | [**CiWorkflowRelationshipsMacOsVersion**](CiWorkflowRelationshipsMacOsVersion.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_workflow_update_request_data_relationships import CiWorkflowUpdateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowUpdateRequestDataRelationships from a JSON string
ci_workflow_update_request_data_relationships_instance = CiWorkflowUpdateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowUpdateRequestDataRelationships.to_json())

# convert the object into a dict
ci_workflow_update_request_data_relationships_dict = ci_workflow_update_request_data_relationships_instance.to_dict()
# create an instance of CiWorkflowUpdateRequestDataRelationships from a dict
ci_workflow_update_request_data_relationships_from_dict = CiWorkflowUpdateRequestDataRelationships.from_dict(ci_workflow_update_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



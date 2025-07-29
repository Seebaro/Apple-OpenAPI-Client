# CiWorkflowCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product** | [**CiWorkflowCreateRequestDataRelationshipsProduct**](CiWorkflowCreateRequestDataRelationshipsProduct.md) |  | 
**repository** | [**CiWorkflowCreateRequestDataRelationshipsRepository**](CiWorkflowCreateRequestDataRelationshipsRepository.md) |  | 
**xcode_version** | [**CiWorkflowCreateRequestDataRelationshipsXcodeVersion**](CiWorkflowCreateRequestDataRelationshipsXcodeVersion.md) |  | 
**mac_os_version** | [**CiWorkflowCreateRequestDataRelationshipsMacOsVersion**](CiWorkflowCreateRequestDataRelationshipsMacOsVersion.md) |  | 

## Example

```python
from openapi_client.models.ci_workflow_create_request_data_relationships import CiWorkflowCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CiWorkflowCreateRequestDataRelationships from a JSON string
ci_workflow_create_request_data_relationships_instance = CiWorkflowCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(CiWorkflowCreateRequestDataRelationships.to_json())

# convert the object into a dict
ci_workflow_create_request_data_relationships_dict = ci_workflow_create_request_data_relationships_instance.to_dict()
# create an instance of CiWorkflowCreateRequestDataRelationships from a dict
ci_workflow_create_request_data_relationships_from_dict = CiWorkflowCreateRequestDataRelationships.from_dict(ci_workflow_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



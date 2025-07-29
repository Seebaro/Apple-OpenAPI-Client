# CiXcodeVersionRelationshipsMacOsVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[CiWorkflowRelationshipsMacOsVersionData]**](CiWorkflowRelationshipsMacOsVersionData.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_xcode_version_relationships_mac_os_versions import CiXcodeVersionRelationshipsMacOsVersions

# TODO update the JSON string below
json = "{}"
# create an instance of CiXcodeVersionRelationshipsMacOsVersions from a JSON string
ci_xcode_version_relationships_mac_os_versions_instance = CiXcodeVersionRelationshipsMacOsVersions.from_json(json)
# print the JSON string representation of the object
print(CiXcodeVersionRelationshipsMacOsVersions.to_json())

# convert the object into a dict
ci_xcode_version_relationships_mac_os_versions_dict = ci_xcode_version_relationships_mac_os_versions_instance.to_dict()
# create an instance of CiXcodeVersionRelationshipsMacOsVersions from a dict
ci_xcode_version_relationships_mac_os_versions_from_dict = CiXcodeVersionRelationshipsMacOsVersions.from_dict(ci_xcode_version_relationships_mac_os_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



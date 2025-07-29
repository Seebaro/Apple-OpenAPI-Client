# CiMacOsVersionRelationshipsXcodeVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[CiMacOsVersionRelationshipsXcodeVersionsDataInner]**](CiMacOsVersionRelationshipsXcodeVersionsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_mac_os_version_relationships_xcode_versions import CiMacOsVersionRelationshipsXcodeVersions

# TODO update the JSON string below
json = "{}"
# create an instance of CiMacOsVersionRelationshipsXcodeVersions from a JSON string
ci_mac_os_version_relationships_xcode_versions_instance = CiMacOsVersionRelationshipsXcodeVersions.from_json(json)
# print the JSON string representation of the object
print(CiMacOsVersionRelationshipsXcodeVersions.to_json())

# convert the object into a dict
ci_mac_os_version_relationships_xcode_versions_dict = ci_mac_os_version_relationships_xcode_versions_instance.to_dict()
# create an instance of CiMacOsVersionRelationshipsXcodeVersions from a dict
ci_mac_os_version_relationships_xcode_versions_from_dict = CiMacOsVersionRelationshipsXcodeVersions.from_dict(ci_mac_os_version_relationships_xcode_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



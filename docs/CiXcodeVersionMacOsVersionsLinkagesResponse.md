# CiXcodeVersionMacOsVersionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiWorkflowRelationshipsMacOsVersionData]**](CiWorkflowRelationshipsMacOsVersionData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_xcode_version_mac_os_versions_linkages_response import CiXcodeVersionMacOsVersionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiXcodeVersionMacOsVersionsLinkagesResponse from a JSON string
ci_xcode_version_mac_os_versions_linkages_response_instance = CiXcodeVersionMacOsVersionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(CiXcodeVersionMacOsVersionsLinkagesResponse.to_json())

# convert the object into a dict
ci_xcode_version_mac_os_versions_linkages_response_dict = ci_xcode_version_mac_os_versions_linkages_response_instance.to_dict()
# create an instance of CiXcodeVersionMacOsVersionsLinkagesResponse from a dict
ci_xcode_version_mac_os_versions_linkages_response_from_dict = CiXcodeVersionMacOsVersionsLinkagesResponse.from_dict(ci_xcode_version_mac_os_versions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



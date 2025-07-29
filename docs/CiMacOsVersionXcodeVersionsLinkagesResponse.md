# CiMacOsVersionXcodeVersionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiMacOsVersionRelationshipsXcodeVersionsDataInner]**](CiMacOsVersionRelationshipsXcodeVersionsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_mac_os_version_xcode_versions_linkages_response import CiMacOsVersionXcodeVersionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiMacOsVersionXcodeVersionsLinkagesResponse from a JSON string
ci_mac_os_version_xcode_versions_linkages_response_instance = CiMacOsVersionXcodeVersionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(CiMacOsVersionXcodeVersionsLinkagesResponse.to_json())

# convert the object into a dict
ci_mac_os_version_xcode_versions_linkages_response_dict = ci_mac_os_version_xcode_versions_linkages_response_instance.to_dict()
# create an instance of CiMacOsVersionXcodeVersionsLinkagesResponse from a dict
ci_mac_os_version_xcode_versions_linkages_response_from_dict = CiMacOsVersionXcodeVersionsLinkagesResponse.from_dict(ci_mac_os_version_xcode_versions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



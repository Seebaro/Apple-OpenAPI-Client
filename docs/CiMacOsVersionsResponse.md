# CiMacOsVersionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiMacOsVersion]**](CiMacOsVersion.md) |  | 
**included** | [**List[CiXcodeVersion]**](CiXcodeVersion.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_mac_os_versions_response import CiMacOsVersionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiMacOsVersionsResponse from a JSON string
ci_mac_os_versions_response_instance = CiMacOsVersionsResponse.from_json(json)
# print the JSON string representation of the object
print(CiMacOsVersionsResponse.to_json())

# convert the object into a dict
ci_mac_os_versions_response_dict = ci_mac_os_versions_response_instance.to_dict()
# create an instance of CiMacOsVersionsResponse from a dict
ci_mac_os_versions_response_from_dict = CiMacOsVersionsResponse.from_dict(ci_mac_os_versions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



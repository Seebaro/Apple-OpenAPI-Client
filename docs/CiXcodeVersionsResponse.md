# CiXcodeVersionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiXcodeVersion]**](CiXcodeVersion.md) |  | 
**included** | [**List[CiMacOsVersion]**](CiMacOsVersion.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_xcode_versions_response import CiXcodeVersionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiXcodeVersionsResponse from a JSON string
ci_xcode_versions_response_instance = CiXcodeVersionsResponse.from_json(json)
# print the JSON string representation of the object
print(CiXcodeVersionsResponse.to_json())

# convert the object into a dict
ci_xcode_versions_response_dict = ci_xcode_versions_response_instance.to_dict()
# create an instance of CiXcodeVersionsResponse from a dict
ci_xcode_versions_response_from_dict = CiXcodeVersionsResponse.from_dict(ci_xcode_versions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiXcodeVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiXcodeVersion**](CiXcodeVersion.md) |  | 
**included** | [**List[CiMacOsVersion]**](CiMacOsVersion.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_xcode_version_response import CiXcodeVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiXcodeVersionResponse from a JSON string
ci_xcode_version_response_instance = CiXcodeVersionResponse.from_json(json)
# print the JSON string representation of the object
print(CiXcodeVersionResponse.to_json())

# convert the object into a dict
ci_xcode_version_response_dict = ci_xcode_version_response_instance.to_dict()
# create an instance of CiXcodeVersionResponse from a dict
ci_xcode_version_response_from_dict = CiXcodeVersionResponse.from_dict(ci_xcode_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



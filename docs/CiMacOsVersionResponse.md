# CiMacOsVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiMacOsVersion**](CiMacOsVersion.md) |  | 
**included** | [**List[CiXcodeVersion]**](CiXcodeVersion.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_mac_os_version_response import CiMacOsVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiMacOsVersionResponse from a JSON string
ci_mac_os_version_response_instance = CiMacOsVersionResponse.from_json(json)
# print the JSON string representation of the object
print(CiMacOsVersionResponse.to_json())

# convert the object into a dict
ci_mac_os_version_response_dict = ci_mac_os_version_response_instance.to_dict()
# create an instance of CiMacOsVersionResponse from a dict
ci_mac_os_version_response_from_dict = CiMacOsVersionResponse.from_dict(ci_mac_os_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



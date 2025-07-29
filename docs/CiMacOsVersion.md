# CiMacOsVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiMacOsVersionAttributes**](CiMacOsVersionAttributes.md) |  | [optional] 
**relationships** | [**CiMacOsVersionRelationships**](CiMacOsVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_mac_os_version import CiMacOsVersion

# TODO update the JSON string below
json = "{}"
# create an instance of CiMacOsVersion from a JSON string
ci_mac_os_version_instance = CiMacOsVersion.from_json(json)
# print the JSON string representation of the object
print(CiMacOsVersion.to_json())

# convert the object into a dict
ci_mac_os_version_dict = ci_mac_os_version_instance.to_dict()
# create an instance of CiMacOsVersion from a dict
ci_mac_os_version_from_dict = CiMacOsVersion.from_dict(ci_mac_os_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



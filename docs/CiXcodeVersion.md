# CiXcodeVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiXcodeVersionAttributes**](CiXcodeVersionAttributes.md) |  | [optional] 
**relationships** | [**CiXcodeVersionRelationships**](CiXcodeVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_xcode_version import CiXcodeVersion

# TODO update the JSON string below
json = "{}"
# create an instance of CiXcodeVersion from a JSON string
ci_xcode_version_instance = CiXcodeVersion.from_json(json)
# print the JSON string representation of the object
print(CiXcodeVersion.to_json())

# convert the object into a dict
ci_xcode_version_dict = ci_xcode_version_instance.to_dict()
# create an instance of CiXcodeVersion from a dict
ci_xcode_version_from_dict = CiXcodeVersion.from_dict(ci_xcode_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



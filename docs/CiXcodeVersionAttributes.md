# CiXcodeVersionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**test_destinations** | [**List[CiXcodeVersionAttributesTestDestinationsInner]**](CiXcodeVersionAttributesTestDestinationsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_xcode_version_attributes import CiXcodeVersionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CiXcodeVersionAttributes from a JSON string
ci_xcode_version_attributes_instance = CiXcodeVersionAttributes.from_json(json)
# print the JSON string representation of the object
print(CiXcodeVersionAttributes.to_json())

# convert the object into a dict
ci_xcode_version_attributes_dict = ci_xcode_version_attributes_instance.to_dict()
# create an instance of CiXcodeVersionAttributes from a dict
ci_xcode_version_attributes_from_dict = CiXcodeVersionAttributes.from_dict(ci_xcode_version_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



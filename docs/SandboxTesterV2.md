# SandboxTesterV2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**SandboxTesterV2Attributes**](SandboxTesterV2Attributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.sandbox_tester_v2 import SandboxTesterV2

# TODO update the JSON string below
json = "{}"
# create an instance of SandboxTesterV2 from a JSON string
sandbox_tester_v2_instance = SandboxTesterV2.from_json(json)
# print the JSON string representation of the object
print(SandboxTesterV2.to_json())

# convert the object into a dict
sandbox_tester_v2_dict = sandbox_tester_v2_instance.to_dict()
# create an instance of SandboxTesterV2 from a dict
sandbox_tester_v2_from_dict = SandboxTesterV2.from_dict(sandbox_tester_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



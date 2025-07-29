# SandboxTesterV2Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SandboxTesterV2**](SandboxTesterV2.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.sandbox_tester_v2_response import SandboxTesterV2Response

# TODO update the JSON string below
json = "{}"
# create an instance of SandboxTesterV2Response from a JSON string
sandbox_tester_v2_response_instance = SandboxTesterV2Response.from_json(json)
# print the JSON string representation of the object
print(SandboxTesterV2Response.to_json())

# convert the object into a dict
sandbox_tester_v2_response_dict = sandbox_tester_v2_response_instance.to_dict()
# create an instance of SandboxTesterV2Response from a dict
sandbox_tester_v2_response_from_dict = SandboxTesterV2Response.from_dict(sandbox_tester_v2_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



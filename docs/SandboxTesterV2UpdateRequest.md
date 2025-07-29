# SandboxTesterV2UpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**SandboxTesterV2UpdateRequestData**](SandboxTesterV2UpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.sandbox_tester_v2_update_request import SandboxTesterV2UpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SandboxTesterV2UpdateRequest from a JSON string
sandbox_tester_v2_update_request_instance = SandboxTesterV2UpdateRequest.from_json(json)
# print the JSON string representation of the object
print(SandboxTesterV2UpdateRequest.to_json())

# convert the object into a dict
sandbox_tester_v2_update_request_dict = sandbox_tester_v2_update_request_instance.to_dict()
# create an instance of SandboxTesterV2UpdateRequest from a dict
sandbox_tester_v2_update_request_from_dict = SandboxTesterV2UpdateRequest.from_dict(sandbox_tester_v2_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



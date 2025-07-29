# SandboxTesterV2UpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**territory** | [**TerritoryCode**](TerritoryCode.md) |  | [optional] 
**interrupt_purchases** | **bool** |  | [optional] 
**subscription_renewal_rate** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.sandbox_tester_v2_update_request_data_attributes import SandboxTesterV2UpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of SandboxTesterV2UpdateRequestDataAttributes from a JSON string
sandbox_tester_v2_update_request_data_attributes_instance = SandboxTesterV2UpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(SandboxTesterV2UpdateRequestDataAttributes.to_json())

# convert the object into a dict
sandbox_tester_v2_update_request_data_attributes_dict = sandbox_tester_v2_update_request_data_attributes_instance.to_dict()
# create an instance of SandboxTesterV2UpdateRequestDataAttributes from a dict
sandbox_tester_v2_update_request_data_attributes_from_dict = SandboxTesterV2UpdateRequestDataAttributes.from_dict(sandbox_tester_v2_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# SandboxTesterV2Attributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**ac_account_name** | **str** |  | [optional] 
**territory** | [**TerritoryCode**](TerritoryCode.md) |  | [optional] 
**apple_pay_compatible** | **bool** |  | [optional] 
**interrupt_purchases** | **bool** |  | [optional] 
**subscription_renewal_rate** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.sandbox_tester_v2_attributes import SandboxTesterV2Attributes

# TODO update the JSON string below
json = "{}"
# create an instance of SandboxTesterV2Attributes from a JSON string
sandbox_tester_v2_attributes_instance = SandboxTesterV2Attributes.from_json(json)
# print the JSON string representation of the object
print(SandboxTesterV2Attributes.to_json())

# convert the object into a dict
sandbox_tester_v2_attributes_dict = sandbox_tester_v2_attributes_instance.to_dict()
# create an instance of SandboxTesterV2Attributes from a dict
sandbox_tester_v2_attributes_from_dict = SandboxTesterV2Attributes.from_dict(sandbox_tester_v2_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



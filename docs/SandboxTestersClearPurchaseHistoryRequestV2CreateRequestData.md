# SandboxTestersClearPurchaseHistoryRequestV2CreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**SandboxTestersClearPurchaseHistoryRequestV2CreateRequestDataRelationships**](SandboxTestersClearPurchaseHistoryRequestV2CreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.sandbox_testers_clear_purchase_history_request_v2_create_request_data import SandboxTestersClearPurchaseHistoryRequestV2CreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of SandboxTestersClearPurchaseHistoryRequestV2CreateRequestData from a JSON string
sandbox_testers_clear_purchase_history_request_v2_create_request_data_instance = SandboxTestersClearPurchaseHistoryRequestV2CreateRequestData.from_json(json)
# print the JSON string representation of the object
print(SandboxTestersClearPurchaseHistoryRequestV2CreateRequestData.to_json())

# convert the object into a dict
sandbox_testers_clear_purchase_history_request_v2_create_request_data_dict = sandbox_testers_clear_purchase_history_request_v2_create_request_data_instance.to_dict()
# create an instance of SandboxTestersClearPurchaseHistoryRequestV2CreateRequestData from a dict
sandbox_testers_clear_purchase_history_request_v2_create_request_data_from_dict = SandboxTestersClearPurchaseHistoryRequestV2CreateRequestData.from_dict(sandbox_testers_clear_purchase_history_request_v2_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# MerchantIdUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MerchantIdUpdateRequestData**](MerchantIdUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.merchant_id_update_request import MerchantIdUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdUpdateRequest from a JSON string
merchant_id_update_request_instance = MerchantIdUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(MerchantIdUpdateRequest.to_json())

# convert the object into a dict
merchant_id_update_request_dict = merchant_id_update_request_instance.to_dict()
# create an instance of MerchantIdUpdateRequest from a dict
merchant_id_update_request_from_dict = MerchantIdUpdateRequest.from_dict(merchant_id_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



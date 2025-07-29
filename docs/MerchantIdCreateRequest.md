# MerchantIdCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MerchantIdCreateRequestData**](MerchantIdCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.merchant_id_create_request import MerchantIdCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdCreateRequest from a JSON string
merchant_id_create_request_instance = MerchantIdCreateRequest.from_json(json)
# print the JSON string representation of the object
print(MerchantIdCreateRequest.to_json())

# convert the object into a dict
merchant_id_create_request_dict = merchant_id_create_request_instance.to_dict()
# create an instance of MerchantIdCreateRequest from a dict
merchant_id_create_request_from_dict = MerchantIdCreateRequest.from_dict(merchant_id_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



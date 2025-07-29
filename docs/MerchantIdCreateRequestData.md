# MerchantIdCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**MerchantIdCreateRequestDataAttributes**](MerchantIdCreateRequestDataAttributes.md) |  | 

## Example

```python
from openapi_client.models.merchant_id_create_request_data import MerchantIdCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdCreateRequestData from a JSON string
merchant_id_create_request_data_instance = MerchantIdCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(MerchantIdCreateRequestData.to_json())

# convert the object into a dict
merchant_id_create_request_data_dict = merchant_id_create_request_data_instance.to_dict()
# create an instance of MerchantIdCreateRequestData from a dict
merchant_id_create_request_data_from_dict = MerchantIdCreateRequestData.from_dict(merchant_id_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



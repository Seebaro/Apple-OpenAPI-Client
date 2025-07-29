# MerchantIdUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BundleIdUpdateRequestDataAttributes**](BundleIdUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.merchant_id_update_request_data import MerchantIdUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdUpdateRequestData from a JSON string
merchant_id_update_request_data_instance = MerchantIdUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(MerchantIdUpdateRequestData.to_json())

# convert the object into a dict
merchant_id_update_request_data_dict = merchant_id_update_request_data_instance.to_dict()
# create an instance of MerchantIdUpdateRequestData from a dict
merchant_id_update_request_data_from_dict = MerchantIdUpdateRequestData.from_dict(merchant_id_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



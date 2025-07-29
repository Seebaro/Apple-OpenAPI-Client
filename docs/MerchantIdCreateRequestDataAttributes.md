# MerchantIdCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**identifier** | **str** |  | 

## Example

```python
from openapi_client.models.merchant_id_create_request_data_attributes import MerchantIdCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdCreateRequestDataAttributes from a JSON string
merchant_id_create_request_data_attributes_instance = MerchantIdCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(MerchantIdCreateRequestDataAttributes.to_json())

# convert the object into a dict
merchant_id_create_request_data_attributes_dict = merchant_id_create_request_data_attributes_instance.to_dict()
# create an instance of MerchantIdCreateRequestDataAttributes from a dict
merchant_id_create_request_data_attributes_from_dict = MerchantIdCreateRequestDataAttributes.from_dict(merchant_id_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



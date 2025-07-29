# MerchantIdAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**identifier** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.merchant_id_attributes import MerchantIdAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdAttributes from a JSON string
merchant_id_attributes_instance = MerchantIdAttributes.from_json(json)
# print the JSON string representation of the object
print(MerchantIdAttributes.to_json())

# convert the object into a dict
merchant_id_attributes_dict = merchant_id_attributes_instance.to_dict()
# create an instance of MerchantIdAttributes from a dict
merchant_id_attributes_from_dict = MerchantIdAttributes.from_dict(merchant_id_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



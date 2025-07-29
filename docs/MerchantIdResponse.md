# MerchantIdResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MerchantId**](MerchantId.md) |  | 
**included** | [**List[Certificate]**](Certificate.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.merchant_id_response import MerchantIdResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdResponse from a JSON string
merchant_id_response_instance = MerchantIdResponse.from_json(json)
# print the JSON string representation of the object
print(MerchantIdResponse.to_json())

# convert the object into a dict
merchant_id_response_dict = merchant_id_response_instance.to_dict()
# create an instance of MerchantIdResponse from a dict
merchant_id_response_from_dict = MerchantIdResponse.from_dict(merchant_id_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



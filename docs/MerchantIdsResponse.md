# MerchantIdsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[MerchantId]**](MerchantId.md) |  | 
**included** | [**List[Certificate]**](Certificate.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.merchant_ids_response import MerchantIdsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdsResponse from a JSON string
merchant_ids_response_instance = MerchantIdsResponse.from_json(json)
# print the JSON string representation of the object
print(MerchantIdsResponse.to_json())

# convert the object into a dict
merchant_ids_response_dict = merchant_ids_response_instance.to_dict()
# create an instance of MerchantIdsResponse from a dict
merchant_ids_response_from_dict = MerchantIdsResponse.from_dict(merchant_ids_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



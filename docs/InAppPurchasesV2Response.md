# InAppPurchasesV2Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[InAppPurchaseV2]**](InAppPurchaseV2.md) |  | 
**included** | [**List[InAppPurchasesV2ResponseIncludedInner]**](InAppPurchasesV2ResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchases_v2_response import InAppPurchasesV2Response

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchasesV2Response from a JSON string
in_app_purchases_v2_response_instance = InAppPurchasesV2Response.from_json(json)
# print the JSON string representation of the object
print(InAppPurchasesV2Response.to_json())

# convert the object into a dict
in_app_purchases_v2_response_dict = in_app_purchases_v2_response_instance.to_dict()
# create an instance of InAppPurchasesV2Response from a dict
in_app_purchases_v2_response_from_dict = InAppPurchasesV2Response.from_dict(in_app_purchases_v2_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



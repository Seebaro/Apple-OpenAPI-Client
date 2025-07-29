# CiProductsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiProduct]**](CiProduct.md) |  | 
**included** | [**List[CiProductsResponseIncludedInner]**](CiProductsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_products_response import CiProductsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductsResponse from a JSON string
ci_products_response_instance = CiProductsResponse.from_json(json)
# print the JSON string representation of the object
print(CiProductsResponse.to_json())

# convert the object into a dict
ci_products_response_dict = ci_products_response_instance.to_dict()
# create an instance of CiProductsResponse from a dict
ci_products_response_from_dict = CiProductsResponse.from_dict(ci_products_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiProductResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiProduct**](CiProduct.md) |  | 
**included** | [**List[CiProductsResponseIncludedInner]**](CiProductsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_product_response import CiProductResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductResponse from a JSON string
ci_product_response_instance = CiProductResponse.from_json(json)
# print the JSON string representation of the object
print(CiProductResponse.to_json())

# convert the object into a dict
ci_product_response_dict = ci_product_response_instance.to_dict()
# create an instance of CiProductResponse from a dict
ci_product_response_from_dict = CiProductResponse.from_dict(ci_product_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



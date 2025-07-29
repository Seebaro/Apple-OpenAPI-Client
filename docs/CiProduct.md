# CiProduct


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiProductAttributes**](CiProductAttributes.md) |  | [optional] 
**relationships** | [**CiProductRelationships**](CiProductRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_product import CiProduct

# TODO update the JSON string below
json = "{}"
# create an instance of CiProduct from a JSON string
ci_product_instance = CiProduct.from_json(json)
# print the JSON string representation of the object
print(CiProduct.to_json())

# convert the object into a dict
ci_product_dict = ci_product_instance.to_dict()
# create an instance of CiProduct from a dict
ci_product_from_dict = CiProduct.from_dict(ci_product_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



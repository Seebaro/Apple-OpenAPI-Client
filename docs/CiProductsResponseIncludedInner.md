# CiProductsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ScmRepositoryAttributes**](ScmRepositoryAttributes.md) |  | [optional] 
**relationships** | [**ScmRepositoryRelationships**](ScmRepositoryRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_products_response_included_inner import CiProductsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductsResponseIncludedInner from a JSON string
ci_products_response_included_inner_instance = CiProductsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(CiProductsResponseIncludedInner.to_json())

# convert the object into a dict
ci_products_response_included_inner_dict = ci_products_response_included_inner_instance.to_dict()
# create an instance of CiProductsResponseIncludedInner from a dict
ci_products_response_included_inner_from_dict = CiProductsResponseIncludedInner.from_dict(ci_products_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



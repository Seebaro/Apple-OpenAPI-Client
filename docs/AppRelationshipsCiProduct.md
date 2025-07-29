# AppRelationshipsCiProduct


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**AppRelationshipsCiProductData**](AppRelationshipsCiProductData.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_ci_product import AppRelationshipsCiProduct

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsCiProduct from a JSON string
app_relationships_ci_product_instance = AppRelationshipsCiProduct.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsCiProduct.to_json())

# convert the object into a dict
app_relationships_ci_product_dict = app_relationships_ci_product_instance.to_dict()
# create an instance of AppRelationshipsCiProduct from a dict
app_relationships_ci_product_from_dict = AppRelationshipsCiProduct.from_dict(app_relationships_ci_product_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



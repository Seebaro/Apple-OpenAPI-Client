# CiProductRelationshipsPrimaryRepositories


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[CiProductRelationshipsPrimaryRepositoriesDataInner]**](CiProductRelationshipsPrimaryRepositoriesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_product_relationships_primary_repositories import CiProductRelationshipsPrimaryRepositories

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductRelationshipsPrimaryRepositories from a JSON string
ci_product_relationships_primary_repositories_instance = CiProductRelationshipsPrimaryRepositories.from_json(json)
# print the JSON string representation of the object
print(CiProductRelationshipsPrimaryRepositories.to_json())

# convert the object into a dict
ci_product_relationships_primary_repositories_dict = ci_product_relationships_primary_repositories_instance.to_dict()
# create an instance of CiProductRelationshipsPrimaryRepositories from a dict
ci_product_relationships_primary_repositories_from_dict = CiProductRelationshipsPrimaryRepositories.from_dict(ci_product_relationships_primary_repositories_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



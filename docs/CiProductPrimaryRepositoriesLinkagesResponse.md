# CiProductPrimaryRepositoriesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiProductRelationshipsPrimaryRepositoriesDataInner]**](CiProductRelationshipsPrimaryRepositoriesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_product_primary_repositories_linkages_response import CiProductPrimaryRepositoriesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductPrimaryRepositoriesLinkagesResponse from a JSON string
ci_product_primary_repositories_linkages_response_instance = CiProductPrimaryRepositoriesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(CiProductPrimaryRepositoriesLinkagesResponse.to_json())

# convert the object into a dict
ci_product_primary_repositories_linkages_response_dict = ci_product_primary_repositories_linkages_response_instance.to_dict()
# create an instance of CiProductPrimaryRepositoriesLinkagesResponse from a dict
ci_product_primary_repositories_linkages_response_from_dict = CiProductPrimaryRepositoriesLinkagesResponse.from_dict(ci_product_primary_repositories_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



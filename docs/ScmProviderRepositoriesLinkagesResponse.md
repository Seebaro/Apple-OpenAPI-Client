# ScmProviderRepositoriesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiProductRelationshipsPrimaryRepositoriesDataInner]**](CiProductRelationshipsPrimaryRepositoriesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_provider_repositories_linkages_response import ScmProviderRepositoriesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmProviderRepositoriesLinkagesResponse from a JSON string
scm_provider_repositories_linkages_response_instance = ScmProviderRepositoriesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(ScmProviderRepositoriesLinkagesResponse.to_json())

# convert the object into a dict
scm_provider_repositories_linkages_response_dict = scm_provider_repositories_linkages_response_instance.to_dict()
# create an instance of ScmProviderRepositoriesLinkagesResponse from a dict
scm_provider_repositories_linkages_response_from_dict = ScmProviderRepositoriesLinkagesResponse.from_dict(scm_provider_repositories_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



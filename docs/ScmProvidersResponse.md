# ScmProvidersResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ScmProvider]**](ScmProvider.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_providers_response import ScmProvidersResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ScmProvidersResponse from a JSON string
scm_providers_response_instance = ScmProvidersResponse.from_json(json)
# print the JSON string representation of the object
print(ScmProvidersResponse.to_json())

# convert the object into a dict
scm_providers_response_dict = scm_providers_response_instance.to_dict()
# create an instance of ScmProvidersResponse from a dict
scm_providers_response_from_dict = ScmProvidersResponse.from_dict(scm_providers_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



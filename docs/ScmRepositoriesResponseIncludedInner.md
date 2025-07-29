# ScmRepositoriesResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ScmGitReferenceAttributes**](ScmGitReferenceAttributes.md) |  | [optional] 
**relationships** | [**ScmGitReferenceRelationships**](ScmGitReferenceRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_repositories_response_included_inner import ScmRepositoriesResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepositoriesResponseIncludedInner from a JSON string
scm_repositories_response_included_inner_instance = ScmRepositoriesResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(ScmRepositoriesResponseIncludedInner.to_json())

# convert the object into a dict
scm_repositories_response_included_inner_dict = scm_repositories_response_included_inner_instance.to_dict()
# create an instance of ScmRepositoriesResponseIncludedInner from a dict
scm_repositories_response_included_inner_from_dict = ScmRepositoriesResponseIncludedInner.from_dict(scm_repositories_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



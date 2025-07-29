# ScmGitReference


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
from openapi_client.models.scm_git_reference import ScmGitReference

# TODO update the JSON string below
json = "{}"
# create an instance of ScmGitReference from a JSON string
scm_git_reference_instance = ScmGitReference.from_json(json)
# print the JSON string representation of the object
print(ScmGitReference.to_json())

# convert the object into a dict
scm_git_reference_dict = scm_git_reference_instance.to_dict()
# create an instance of ScmGitReference from a dict
scm_git_reference_from_dict = ScmGitReference.from_dict(scm_git_reference_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



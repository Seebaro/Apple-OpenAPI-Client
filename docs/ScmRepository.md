# ScmRepository


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
from openapi_client.models.scm_repository import ScmRepository

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepository from a JSON string
scm_repository_instance = ScmRepository.from_json(json)
# print the JSON string representation of the object
print(ScmRepository.to_json())

# convert the object into a dict
scm_repository_dict = scm_repository_instance.to_dict()
# create an instance of ScmRepository from a dict
scm_repository_from_dict = ScmRepository.from_dict(scm_repository_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



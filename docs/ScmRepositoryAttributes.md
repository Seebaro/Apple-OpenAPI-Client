# ScmRepositoryAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**last_accessed_date** | **datetime** |  | [optional] 
**http_clone_url** | **str** |  | [optional] 
**ssh_clone_url** | **str** |  | [optional] 
**owner_name** | **str** |  | [optional] 
**repository_name** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.scm_repository_attributes import ScmRepositoryAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ScmRepositoryAttributes from a JSON string
scm_repository_attributes_instance = ScmRepositoryAttributes.from_json(json)
# print the JSON string representation of the object
print(ScmRepositoryAttributes.to_json())

# convert the object into a dict
scm_repository_attributes_dict = scm_repository_attributes_instance.to_dict()
# create an instance of ScmRepositoryAttributes from a dict
scm_repository_attributes_from_dict = ScmRepositoryAttributes.from_dict(scm_repository_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



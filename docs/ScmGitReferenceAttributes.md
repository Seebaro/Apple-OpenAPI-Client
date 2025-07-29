# ScmGitReferenceAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**canonical_name** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**kind** | [**CiGitRefKind**](CiGitRefKind.md) |  | [optional] 

## Example

```python
from openapi_client.models.scm_git_reference_attributes import ScmGitReferenceAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ScmGitReferenceAttributes from a JSON string
scm_git_reference_attributes_instance = ScmGitReferenceAttributes.from_json(json)
# print the JSON string representation of the object
print(ScmGitReferenceAttributes.to_json())

# convert the object into a dict
scm_git_reference_attributes_dict = scm_git_reference_attributes_instance.to_dict()
# create an instance of ScmGitReferenceAttributes from a dict
scm_git_reference_attributes_from_dict = ScmGitReferenceAttributes.from_dict(scm_git_reference_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



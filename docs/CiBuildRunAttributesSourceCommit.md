# CiBuildRunAttributesSourceCommit


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**commit_sha** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**author** | [**CiGitUser**](CiGitUser.md) |  | [optional] 
**committer** | [**CiGitUser**](CiGitUser.md) |  | [optional] 
**web_url** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_run_attributes_source_commit import CiBuildRunAttributesSourceCommit

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRunAttributesSourceCommit from a JSON string
ci_build_run_attributes_source_commit_instance = CiBuildRunAttributesSourceCommit.from_json(json)
# print the JSON string representation of the object
print(CiBuildRunAttributesSourceCommit.to_json())

# convert the object into a dict
ci_build_run_attributes_source_commit_dict = ci_build_run_attributes_source_commit_instance.to_dict()
# create an instance of CiBuildRunAttributesSourceCommit from a dict
ci_build_run_attributes_source_commit_from_dict = CiBuildRunAttributesSourceCommit.from_dict(ci_build_run_attributes_source_commit_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiGitUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | [optional] 
**avatar_url** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_git_user import CiGitUser

# TODO update the JSON string below
json = "{}"
# create an instance of CiGitUser from a JSON string
ci_git_user_instance = CiGitUser.from_json(json)
# print the JSON string representation of the object
print(CiGitUser.to_json())

# convert the object into a dict
ci_git_user_dict = ci_git_user_instance.to_dict()
# create an instance of CiGitUser from a dict
ci_git_user_from_dict = CiGitUser.from_dict(ci_git_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



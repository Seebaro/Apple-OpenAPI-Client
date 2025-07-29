# CiBranchStartCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**CiBranchPatterns**](CiBranchPatterns.md) |  | [optional] 
**files_and_folders_rule** | [**CiFilesAndFoldersRule**](CiFilesAndFoldersRule.md) |  | [optional] 
**auto_cancel** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.ci_branch_start_condition import CiBranchStartCondition

# TODO update the JSON string below
json = "{}"
# create an instance of CiBranchStartCondition from a JSON string
ci_branch_start_condition_instance = CiBranchStartCondition.from_json(json)
# print the JSON string representation of the object
print(CiBranchStartCondition.to_json())

# convert the object into a dict
ci_branch_start_condition_dict = ci_branch_start_condition_instance.to_dict()
# create an instance of CiBranchStartCondition from a dict
ci_branch_start_condition_from_dict = CiBranchStartCondition.from_dict(ci_branch_start_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



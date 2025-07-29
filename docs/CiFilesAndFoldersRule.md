# CiFilesAndFoldersRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**mode** | **str** |  | [optional] 
**matchers** | [**List[CiStartConditionFileMatcher]**](CiStartConditionFileMatcher.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_files_and_folders_rule import CiFilesAndFoldersRule

# TODO update the JSON string below
json = "{}"
# create an instance of CiFilesAndFoldersRule from a JSON string
ci_files_and_folders_rule_instance = CiFilesAndFoldersRule.from_json(json)
# print the JSON string representation of the object
print(CiFilesAndFoldersRule.to_json())

# convert the object into a dict
ci_files_and_folders_rule_dict = ci_files_and_folders_rule_instance.to_dict()
# create an instance of CiFilesAndFoldersRule from a dict
ci_files_and_folders_rule_from_dict = CiFilesAndFoldersRule.from_dict(ci_files_and_folders_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiTagStartCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**CiTagPatterns**](CiTagPatterns.md) |  | [optional] 
**files_and_folders_rule** | [**CiFilesAndFoldersRule**](CiFilesAndFoldersRule.md) |  | [optional] 
**auto_cancel** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.ci_tag_start_condition import CiTagStartCondition

# TODO update the JSON string below
json = "{}"
# create an instance of CiTagStartCondition from a JSON string
ci_tag_start_condition_instance = CiTagStartCondition.from_json(json)
# print the JSON string representation of the object
print(CiTagStartCondition.to_json())

# convert the object into a dict
ci_tag_start_condition_dict = ci_tag_start_condition_instance.to_dict()
# create an instance of CiTagStartCondition from a dict
ci_tag_start_condition_from_dict = CiTagStartCondition.from_dict(ci_tag_start_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



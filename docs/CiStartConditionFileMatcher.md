# CiStartConditionFileMatcher


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**directory** | **str** |  | [optional] 
**file_extension** | **str** |  | [optional] 
**file_name** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.ci_start_condition_file_matcher import CiStartConditionFileMatcher

# TODO update the JSON string below
json = "{}"
# create an instance of CiStartConditionFileMatcher from a JSON string
ci_start_condition_file_matcher_instance = CiStartConditionFileMatcher.from_json(json)
# print the JSON string representation of the object
print(CiStartConditionFileMatcher.to_json())

# convert the object into a dict
ci_start_condition_file_matcher_dict = ci_start_condition_file_matcher_instance.to_dict()
# create an instance of CiStartConditionFileMatcher from a dict
ci_start_condition_file_matcher_from_dict = CiStartConditionFileMatcher.from_dict(ci_start_condition_file_matcher_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



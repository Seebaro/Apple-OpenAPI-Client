# CiManualBranchStartCondition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**CiBranchPatterns**](CiBranchPatterns.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_manual_branch_start_condition import CiManualBranchStartCondition

# TODO update the JSON string below
json = "{}"
# create an instance of CiManualBranchStartCondition from a JSON string
ci_manual_branch_start_condition_instance = CiManualBranchStartCondition.from_json(json)
# print the JSON string representation of the object
print(CiManualBranchStartCondition.to_json())

# convert the object into a dict
ci_manual_branch_start_condition_dict = ci_manual_branch_start_condition_instance.to_dict()
# create an instance of CiManualBranchStartCondition from a dict
ci_manual_branch_start_condition_from_dict = CiManualBranchStartCondition.from_dict(ci_manual_branch_start_condition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiBranchPatterns


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_all_match** | **bool** |  | [optional] 
**patterns** | [**List[CiBranchPatternsPatternsInner]**](CiBranchPatternsPatternsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_branch_patterns import CiBranchPatterns

# TODO update the JSON string below
json = "{}"
# create an instance of CiBranchPatterns from a JSON string
ci_branch_patterns_instance = CiBranchPatterns.from_json(json)
# print the JSON string representation of the object
print(CiBranchPatterns.to_json())

# convert the object into a dict
ci_branch_patterns_dict = ci_branch_patterns_instance.to_dict()
# create an instance of CiBranchPatterns from a dict
ci_branch_patterns_from_dict = CiBranchPatterns.from_dict(ci_branch_patterns_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



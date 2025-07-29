# CiTagPatterns


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_all_match** | **bool** |  | [optional] 
**patterns** | [**List[CiBranchPatternsPatternsInner]**](CiBranchPatternsPatternsInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_tag_patterns import CiTagPatterns

# TODO update the JSON string below
json = "{}"
# create an instance of CiTagPatterns from a JSON string
ci_tag_patterns_instance = CiTagPatterns.from_json(json)
# print the JSON string representation of the object
print(CiTagPatterns.to_json())

# convert the object into a dict
ci_tag_patterns_dict = ci_tag_patterns_instance.to_dict()
# create an instance of CiTagPatterns from a dict
ci_tag_patterns_from_dict = CiTagPatterns.from_dict(ci_tag_patterns_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



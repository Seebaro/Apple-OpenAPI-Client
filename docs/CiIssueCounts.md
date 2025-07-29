# CiIssueCounts


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**analyzer_warnings** | **int** |  | [optional] 
**errors** | **int** |  | [optional] 
**test_failures** | **int** |  | [optional] 
**warnings** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.ci_issue_counts import CiIssueCounts

# TODO update the JSON string below
json = "{}"
# create an instance of CiIssueCounts from a JSON string
ci_issue_counts_instance = CiIssueCounts.from_json(json)
# print the JSON string representation of the object
print(CiIssueCounts.to_json())

# convert the object into a dict
ci_issue_counts_dict = ci_issue_counts_instance.to_dict()
# create an instance of CiIssueCounts from a dict
ci_issue_counts_from_dict = CiIssueCounts.from_dict(ci_issue_counts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



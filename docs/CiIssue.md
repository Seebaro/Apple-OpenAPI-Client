# CiIssue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiIssueAttributes**](CiIssueAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_issue import CiIssue

# TODO update the JSON string below
json = "{}"
# create an instance of CiIssue from a JSON string
ci_issue_instance = CiIssue.from_json(json)
# print the JSON string representation of the object
print(CiIssue.to_json())

# convert the object into a dict
ci_issue_dict = ci_issue_instance.to_dict()
# create an instance of CiIssue from a dict
ci_issue_from_dict = CiIssue.from_dict(ci_issue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CiIssueResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CiIssue**](CiIssue.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.ci_issue_response import CiIssueResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiIssueResponse from a JSON string
ci_issue_response_instance = CiIssueResponse.from_json(json)
# print the JSON string representation of the object
print(CiIssueResponse.to_json())

# convert the object into a dict
ci_issue_response_dict = ci_issue_response_instance.to_dict()
# create an instance of CiIssueResponse from a dict
ci_issue_response_from_dict = CiIssueResponse.from_dict(ci_issue_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



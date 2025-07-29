# CiIssuesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiIssue]**](CiIssue.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_issues_response import CiIssuesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiIssuesResponse from a JSON string
ci_issues_response_instance = CiIssuesResponse.from_json(json)
# print the JSON string representation of the object
print(CiIssuesResponse.to_json())

# convert the object into a dict
ci_issues_response_dict = ci_issues_response_instance.to_dict()
# create an instance of CiIssuesResponse from a dict
ci_issues_response_from_dict = CiIssuesResponse.from_dict(ci_issues_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



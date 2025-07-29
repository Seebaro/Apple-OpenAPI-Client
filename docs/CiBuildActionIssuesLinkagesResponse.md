# CiBuildActionIssuesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CiBuildActionIssuesLinkagesResponseDataInner]**](CiBuildActionIssuesLinkagesResponseDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_action_issues_linkages_response import CiBuildActionIssuesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildActionIssuesLinkagesResponse from a JSON string
ci_build_action_issues_linkages_response_instance = CiBuildActionIssuesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(CiBuildActionIssuesLinkagesResponse.to_json())

# convert the object into a dict
ci_build_action_issues_linkages_response_dict = ci_build_action_issues_linkages_response_instance.to_dict()
# create an instance of CiBuildActionIssuesLinkagesResponse from a dict
ci_build_action_issues_linkages_response_from_dict = CiBuildActionIssuesLinkagesResponse.from_dict(ci_build_action_issues_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



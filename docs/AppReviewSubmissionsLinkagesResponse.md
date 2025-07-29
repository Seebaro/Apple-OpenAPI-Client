# AppReviewSubmissionsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppRelationshipsReviewSubmissionsDataInner]**](AppRelationshipsReviewSubmissionsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_review_submissions_linkages_response import AppReviewSubmissionsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppReviewSubmissionsLinkagesResponse from a JSON string
app_review_submissions_linkages_response_instance = AppReviewSubmissionsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppReviewSubmissionsLinkagesResponse.to_json())

# convert the object into a dict
app_review_submissions_linkages_response_dict = app_review_submissions_linkages_response_instance.to_dict()
# create an instance of AppReviewSubmissionsLinkagesResponse from a dict
app_review_submissions_linkages_response_from_dict = AppReviewSubmissionsLinkagesResponse.from_dict(app_review_submissions_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



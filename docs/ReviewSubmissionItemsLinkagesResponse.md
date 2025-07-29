# ReviewSubmissionItemsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ReviewSubmissionRelationshipsItemsDataInner]**](ReviewSubmissionRelationshipsItemsDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_items_linkages_response import ReviewSubmissionItemsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemsLinkagesResponse from a JSON string
review_submission_items_linkages_response_instance = ReviewSubmissionItemsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemsLinkagesResponse.to_json())

# convert the object into a dict
review_submission_items_linkages_response_dict = review_submission_items_linkages_response_instance.to_dict()
# create an instance of ReviewSubmissionItemsLinkagesResponse from a dict
review_submission_items_linkages_response_from_dict = ReviewSubmissionItemsLinkagesResponse.from_dict(review_submission_items_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



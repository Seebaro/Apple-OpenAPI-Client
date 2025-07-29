# ReviewSubmissionItemsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ReviewSubmissionItem]**](ReviewSubmissionItem.md) |  | 
**included** | [**List[ReviewSubmissionItemsResponseIncludedInner]**](ReviewSubmissionItemsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_items_response import ReviewSubmissionItemsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemsResponse from a JSON string
review_submission_items_response_instance = ReviewSubmissionItemsResponse.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemsResponse.to_json())

# convert the object into a dict
review_submission_items_response_dict = review_submission_items_response_instance.to_dict()
# create an instance of ReviewSubmissionItemsResponse from a dict
review_submission_items_response_from_dict = ReviewSubmissionItemsResponse.from_dict(review_submission_items_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



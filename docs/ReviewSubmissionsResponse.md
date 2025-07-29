# ReviewSubmissionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ReviewSubmission]**](ReviewSubmission.md) |  | 
**included** | [**List[ReviewSubmissionsResponseIncludedInner]**](ReviewSubmissionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submissions_response import ReviewSubmissionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionsResponse from a JSON string
review_submissions_response_instance = ReviewSubmissionsResponse.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionsResponse.to_json())

# convert the object into a dict
review_submissions_response_dict = review_submissions_response_instance.to_dict()
# create an instance of ReviewSubmissionsResponse from a dict
review_submissions_response_from_dict = ReviewSubmissionsResponse.from_dict(review_submissions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



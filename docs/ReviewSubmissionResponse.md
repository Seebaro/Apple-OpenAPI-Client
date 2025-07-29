# ReviewSubmissionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ReviewSubmission**](ReviewSubmission.md) |  | 
**included** | [**List[ReviewSubmissionsResponseIncludedInner]**](ReviewSubmissionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.review_submission_response import ReviewSubmissionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionResponse from a JSON string
review_submission_response_instance = ReviewSubmissionResponse.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionResponse.to_json())

# convert the object into a dict
review_submission_response_dict = review_submission_response_instance.to_dict()
# create an instance of ReviewSubmissionResponse from a dict
review_submission_response_from_dict = ReviewSubmissionResponse.from_dict(review_submission_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



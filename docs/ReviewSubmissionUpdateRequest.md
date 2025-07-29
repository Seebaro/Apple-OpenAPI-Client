# ReviewSubmissionUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ReviewSubmissionUpdateRequestData**](ReviewSubmissionUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.review_submission_update_request import ReviewSubmissionUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionUpdateRequest from a JSON string
review_submission_update_request_instance = ReviewSubmissionUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionUpdateRequest.to_json())

# convert the object into a dict
review_submission_update_request_dict = review_submission_update_request_instance.to_dict()
# create an instance of ReviewSubmissionUpdateRequest from a dict
review_submission_update_request_from_dict = ReviewSubmissionUpdateRequest.from_dict(review_submission_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



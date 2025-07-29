# ReviewSubmissionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ReviewSubmissionCreateRequestData**](ReviewSubmissionCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.review_submission_create_request import ReviewSubmissionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionCreateRequest from a JSON string
review_submission_create_request_instance = ReviewSubmissionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionCreateRequest.to_json())

# convert the object into a dict
review_submission_create_request_dict = review_submission_create_request_instance.to_dict()
# create an instance of ReviewSubmissionCreateRequest from a dict
review_submission_create_request_from_dict = ReviewSubmissionCreateRequest.from_dict(review_submission_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



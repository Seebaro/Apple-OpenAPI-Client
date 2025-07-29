# ReviewSubmissionItemCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ReviewSubmissionItemCreateRequestData**](ReviewSubmissionItemCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.review_submission_item_create_request import ReviewSubmissionItemCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemCreateRequest from a JSON string
review_submission_item_create_request_instance = ReviewSubmissionItemCreateRequest.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemCreateRequest.to_json())

# convert the object into a dict
review_submission_item_create_request_dict = review_submission_item_create_request_instance.to_dict()
# create an instance of ReviewSubmissionItemCreateRequest from a dict
review_submission_item_create_request_from_dict = ReviewSubmissionItemCreateRequest.from_dict(review_submission_item_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



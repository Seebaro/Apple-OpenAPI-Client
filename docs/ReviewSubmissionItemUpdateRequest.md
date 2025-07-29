# ReviewSubmissionItemUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ReviewSubmissionItemUpdateRequestData**](ReviewSubmissionItemUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.review_submission_item_update_request import ReviewSubmissionItemUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemUpdateRequest from a JSON string
review_submission_item_update_request_instance = ReviewSubmissionItemUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemUpdateRequest.to_json())

# convert the object into a dict
review_submission_item_update_request_dict = review_submission_item_update_request_instance.to_dict()
# create an instance of ReviewSubmissionItemUpdateRequest from a dict
review_submission_item_update_request_from_dict = ReviewSubmissionItemUpdateRequest.from_dict(review_submission_item_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



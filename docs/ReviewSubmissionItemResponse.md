# ReviewSubmissionItemResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ReviewSubmissionItem**](ReviewSubmissionItem.md) |  | 
**included** | [**List[ReviewSubmissionItemsResponseIncludedInner]**](ReviewSubmissionItemsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.review_submission_item_response import ReviewSubmissionItemResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemResponse from a JSON string
review_submission_item_response_instance = ReviewSubmissionItemResponse.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemResponse.to_json())

# convert the object into a dict
review_submission_item_response_dict = review_submission_item_response_instance.to_dict()
# create an instance of ReviewSubmissionItemResponse from a dict
review_submission_item_response_from_dict = ReviewSubmissionItemResponse.from_dict(review_submission_item_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



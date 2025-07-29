# ReviewSubmissionItemCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**ReviewSubmissionItemCreateRequestDataRelationships**](ReviewSubmissionItemCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.review_submission_item_create_request_data import ReviewSubmissionItemCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemCreateRequestData from a JSON string
review_submission_item_create_request_data_instance = ReviewSubmissionItemCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemCreateRequestData.to_json())

# convert the object into a dict
review_submission_item_create_request_data_dict = review_submission_item_create_request_data_instance.to_dict()
# create an instance of ReviewSubmissionItemCreateRequestData from a dict
review_submission_item_create_request_data_from_dict = ReviewSubmissionItemCreateRequestData.from_dict(review_submission_item_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



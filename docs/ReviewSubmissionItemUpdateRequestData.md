# ReviewSubmissionItemUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ReviewSubmissionItemUpdateRequestDataAttributes**](ReviewSubmissionItemUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_item_update_request_data import ReviewSubmissionItemUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemUpdateRequestData from a JSON string
review_submission_item_update_request_data_instance = ReviewSubmissionItemUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemUpdateRequestData.to_json())

# convert the object into a dict
review_submission_item_update_request_data_dict = review_submission_item_update_request_data_instance.to_dict()
# create an instance of ReviewSubmissionItemUpdateRequestData from a dict
review_submission_item_update_request_data_from_dict = ReviewSubmissionItemUpdateRequestData.from_dict(review_submission_item_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ReviewSubmissionItemUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**resolved** | **bool** |  | [optional] 
**removed** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_item_update_request_data_attributes import ReviewSubmissionItemUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemUpdateRequestDataAttributes from a JSON string
review_submission_item_update_request_data_attributes_instance = ReviewSubmissionItemUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemUpdateRequestDataAttributes.to_json())

# convert the object into a dict
review_submission_item_update_request_data_attributes_dict = review_submission_item_update_request_data_attributes_instance.to_dict()
# create an instance of ReviewSubmissionItemUpdateRequestDataAttributes from a dict
review_submission_item_update_request_data_attributes_from_dict = ReviewSubmissionItemUpdateRequestDataAttributes.from_dict(review_submission_item_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



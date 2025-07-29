# ReviewSubmissionUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | [**Platform**](Platform.md) |  | [optional] 
**submitted** | **bool** |  | [optional] 
**canceled** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_update_request_data_attributes import ReviewSubmissionUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionUpdateRequestDataAttributes from a JSON string
review_submission_update_request_data_attributes_instance = ReviewSubmissionUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionUpdateRequestDataAttributes.to_json())

# convert the object into a dict
review_submission_update_request_data_attributes_dict = review_submission_update_request_data_attributes_instance.to_dict()
# create an instance of ReviewSubmissionUpdateRequestDataAttributes from a dict
review_submission_update_request_data_attributes_from_dict = ReviewSubmissionUpdateRequestDataAttributes.from_dict(review_submission_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



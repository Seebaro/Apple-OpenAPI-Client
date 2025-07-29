# ReviewSubmissionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | [**Platform**](Platform.md) |  | [optional] 
**submitted_date** | **datetime** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_attributes import ReviewSubmissionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionAttributes from a JSON string
review_submission_attributes_instance = ReviewSubmissionAttributes.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionAttributes.to_json())

# convert the object into a dict
review_submission_attributes_dict = review_submission_attributes_instance.to_dict()
# create an instance of ReviewSubmissionAttributes from a dict
review_submission_attributes_from_dict = ReviewSubmissionAttributes.from_dict(review_submission_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



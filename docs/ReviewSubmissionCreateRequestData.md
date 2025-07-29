# ReviewSubmissionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**ReviewSubmissionCreateRequestDataAttributes**](ReviewSubmissionCreateRequestDataAttributes.md) |  | [optional] 
**relationships** | [**AccessibilityDeclarationCreateRequestDataRelationships**](AccessibilityDeclarationCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.review_submission_create_request_data import ReviewSubmissionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionCreateRequestData from a JSON string
review_submission_create_request_data_instance = ReviewSubmissionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionCreateRequestData.to_json())

# convert the object into a dict
review_submission_create_request_data_dict = review_submission_create_request_data_instance.to_dict()
# create an instance of ReviewSubmissionCreateRequestData from a dict
review_submission_create_request_data_from_dict = ReviewSubmissionCreateRequestData.from_dict(review_submission_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# ReviewSubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ReviewSubmissionAttributes**](ReviewSubmissionAttributes.md) |  | [optional] 
**relationships** | [**ReviewSubmissionRelationships**](ReviewSubmissionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission import ReviewSubmission

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmission from a JSON string
review_submission_instance = ReviewSubmission.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmission.to_json())

# convert the object into a dict
review_submission_dict = review_submission_instance.to_dict()
# create an instance of ReviewSubmission from a dict
review_submission_from_dict = ReviewSubmission.from_dict(review_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



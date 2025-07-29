# ReviewSubmissionItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ReviewSubmissionItemAttributes**](ReviewSubmissionItemAttributes.md) |  | [optional] 
**relationships** | [**ReviewSubmissionItemRelationships**](ReviewSubmissionItemRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_item import ReviewSubmissionItem

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItem from a JSON string
review_submission_item_instance = ReviewSubmissionItem.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItem.to_json())

# convert the object into a dict
review_submission_item_dict = review_submission_item_instance.to_dict()
# create an instance of ReviewSubmissionItem from a dict
review_submission_item_from_dict = ReviewSubmissionItem.from_dict(review_submission_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



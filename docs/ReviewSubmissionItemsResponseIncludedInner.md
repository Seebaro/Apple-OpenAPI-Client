# ReviewSubmissionItemsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppEventAttributes**](AppEventAttributes.md) |  | [optional] 
**relationships** | [**AppEventRelationships**](AppEventRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_items_response_included_inner import ReviewSubmissionItemsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemsResponseIncludedInner from a JSON string
review_submission_items_response_included_inner_instance = ReviewSubmissionItemsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemsResponseIncludedInner.to_json())

# convert the object into a dict
review_submission_items_response_included_inner_dict = review_submission_items_response_included_inner_instance.to_dict()
# create an instance of ReviewSubmissionItemsResponseIncludedInner from a dict
review_submission_items_response_included_inner_from_dict = ReviewSubmissionItemsResponseIncludedInner.from_dict(review_submission_items_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



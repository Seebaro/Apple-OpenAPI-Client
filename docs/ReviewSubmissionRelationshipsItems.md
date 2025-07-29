# ReviewSubmissionRelationshipsItems


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[ReviewSubmissionRelationshipsItemsDataInner]**](ReviewSubmissionRelationshipsItemsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_relationships_items import ReviewSubmissionRelationshipsItems

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionRelationshipsItems from a JSON string
review_submission_relationships_items_instance = ReviewSubmissionRelationshipsItems.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionRelationshipsItems.to_json())

# convert the object into a dict
review_submission_relationships_items_dict = review_submission_relationships_items_instance.to_dict()
# create an instance of ReviewSubmissionRelationshipsItems from a dict
review_submission_relationships_items_from_dict = ReviewSubmissionRelationshipsItems.from_dict(review_submission_relationships_items_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AppRelationshipsReviewSubmissions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppRelationshipsReviewSubmissionsDataInner]**](AppRelationshipsReviewSubmissionsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships_review_submissions import AppRelationshipsReviewSubmissions

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationshipsReviewSubmissions from a JSON string
app_relationships_review_submissions_instance = AppRelationshipsReviewSubmissions.from_json(json)
# print the JSON string representation of the object
print(AppRelationshipsReviewSubmissions.to_json())

# convert the object into a dict
app_relationships_review_submissions_dict = app_relationships_review_submissions_instance.to_dict()
# create an instance of AppRelationshipsReviewSubmissions from a dict
app_relationships_review_submissions_from_dict = AppRelationshipsReviewSubmissions.from_dict(app_relationships_review_submissions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



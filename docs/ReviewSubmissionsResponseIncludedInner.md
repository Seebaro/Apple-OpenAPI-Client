# ReviewSubmissionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**ActorAttributes**](ActorAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionRelationships**](AppStoreVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submissions_response_included_inner import ReviewSubmissionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionsResponseIncludedInner from a JSON string
review_submissions_response_included_inner_instance = ReviewSubmissionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionsResponseIncludedInner.to_json())

# convert the object into a dict
review_submissions_response_included_inner_dict = review_submissions_response_included_inner_instance.to_dict()
# create an instance of ReviewSubmissionsResponseIncludedInner from a dict
review_submissions_response_included_inner_from_dict = ReviewSubmissionsResponseIncludedInner.from_dict(review_submissions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



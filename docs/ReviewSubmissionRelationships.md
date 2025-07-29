# ReviewSubmissionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**items** | [**ReviewSubmissionRelationshipsItems**](ReviewSubmissionRelationshipsItems.md) |  | [optional] 
**app_store_version_for_review** | [**AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**submitted_by_actor** | [**NominationRelationshipsCreatedByActor**](NominationRelationshipsCreatedByActor.md) |  | [optional] 
**last_updated_by_actor** | [**NominationRelationshipsCreatedByActor**](NominationRelationshipsCreatedByActor.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_relationships import ReviewSubmissionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionRelationships from a JSON string
review_submission_relationships_instance = ReviewSubmissionRelationships.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionRelationships.to_json())

# convert the object into a dict
review_submission_relationships_dict = review_submission_relationships_instance.to_dict()
# create an instance of ReviewSubmissionRelationships from a dict
review_submission_relationships_from_dict = ReviewSubmissionRelationships.from_dict(review_submission_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



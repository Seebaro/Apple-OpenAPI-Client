# ReviewSubmissionItemRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_store_version** | [**AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**app_custom_product_page_version** | [**AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersion**](AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersion.md) |  | [optional] 
**app_store_version_experiment** | [**AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment**](AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment.md) |  | [optional] 
**app_store_version_experiment_v2** | [**AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment**](AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment.md) |  | [optional] 
**app_event** | [**AppEventLocalizationRelationshipsAppEvent**](AppEventLocalizationRelationshipsAppEvent.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_item_relationships import ReviewSubmissionItemRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemRelationships from a JSON string
review_submission_item_relationships_instance = ReviewSubmissionItemRelationships.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemRelationships.to_json())

# convert the object into a dict
review_submission_item_relationships_dict = review_submission_item_relationships_instance.to_dict()
# create an instance of ReviewSubmissionItemRelationships from a dict
review_submission_item_relationships_from_dict = ReviewSubmissionItemRelationships.from_dict(review_submission_item_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



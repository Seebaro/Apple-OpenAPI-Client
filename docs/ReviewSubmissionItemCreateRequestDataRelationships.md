# ReviewSubmissionItemCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**review_submission** | [**ReviewSubmissionItemCreateRequestDataRelationshipsReviewSubmission**](ReviewSubmissionItemCreateRequestDataRelationshipsReviewSubmission.md) |  | 
**app_store_version** | [**AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceCreateRequestDataRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**app_custom_product_page_version** | [**AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersion**](AppCustomProductPageLocalizationRelationshipsAppCustomProductPageVersion.md) |  | [optional] 
**app_store_version_experiment** | [**AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment**](AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment.md) |  | [optional] 
**app_store_version_experiment_v2** | [**AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment**](AppStoreVersionExperimentTreatmentRelationshipsAppStoreVersionExperiment.md) |  | [optional] 
**app_event** | [**AppEventLocalizationRelationshipsAppEvent**](AppEventLocalizationRelationshipsAppEvent.md) |  | [optional] 

## Example

```python
from openapi_client.models.review_submission_item_create_request_data_relationships import ReviewSubmissionItemCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of ReviewSubmissionItemCreateRequestDataRelationships from a JSON string
review_submission_item_create_request_data_relationships_instance = ReviewSubmissionItemCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(ReviewSubmissionItemCreateRequestDataRelationships.to_json())

# convert the object into a dict
review_submission_item_create_request_data_relationships_dict = review_submission_item_create_request_data_relationships_instance.to_dict()
# create an instance of ReviewSubmissionItemCreateRequestDataRelationships from a dict
review_submission_item_create_request_data_relationships_from_dict = ReviewSubmissionItemCreateRequestDataRelationships.from_dict(review_submission_item_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



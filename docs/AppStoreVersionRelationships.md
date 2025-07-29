# AppStoreVersionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**age_rating_declaration** | [**AppStoreVersionRelationshipsAgeRatingDeclaration**](AppStoreVersionRelationshipsAgeRatingDeclaration.md) |  | [optional] 
**app_store_version_localizations** | [**AppStoreVersionRelationshipsAppStoreVersionLocalizations**](AppStoreVersionRelationshipsAppStoreVersionLocalizations.md) |  | [optional] 
**build** | [**AppStoreVersionRelationshipsBuild**](AppStoreVersionRelationshipsBuild.md) |  | [optional] 
**app_store_version_phased_release** | [**AppStoreVersionRelationshipsAppStoreVersionPhasedRelease**](AppStoreVersionRelationshipsAppStoreVersionPhasedRelease.md) |  | [optional] 
**game_center_app_version** | [**AppStoreVersionRelationshipsGameCenterAppVersion**](AppStoreVersionRelationshipsGameCenterAppVersion.md) |  | [optional] 
**routing_app_coverage** | [**AppStoreVersionRelationshipsRoutingAppCoverage**](AppStoreVersionRelationshipsRoutingAppCoverage.md) |  | [optional] 
**app_store_review_detail** | [**AppStoreVersionRelationshipsAppStoreReviewDetail**](AppStoreVersionRelationshipsAppStoreReviewDetail.md) |  | [optional] 
**app_store_version_submission** | [**AppStoreVersionRelationshipsAppStoreVersionSubmission**](AppStoreVersionRelationshipsAppStoreVersionSubmission.md) |  | [optional] 
**app_clip_default_experience** | [**AppStoreVersionRelationshipsAppClipDefaultExperience**](AppStoreVersionRelationshipsAppClipDefaultExperience.md) |  | [optional] 
**app_store_version_experiments** | [**AppStoreVersionRelationshipsAppStoreVersionExperiments**](AppStoreVersionRelationshipsAppStoreVersionExperiments.md) |  | [optional] 
**app_store_version_experiments_v2** | [**AppStoreVersionRelationshipsAppStoreVersionExperiments**](AppStoreVersionRelationshipsAppStoreVersionExperiments.md) |  | [optional] 
**customer_reviews** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**alternative_distribution_package** | [**AppStoreVersionRelationshipsAlternativeDistributionPackage**](AppStoreVersionRelationshipsAlternativeDistributionPackage.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_relationships import AppStoreVersionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionRelationships from a JSON string
app_store_version_relationships_instance = AppStoreVersionRelationships.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionRelationships.to_json())

# convert the object into a dict
app_store_version_relationships_dict = app_store_version_relationships_instance.to_dict()
# create an instance of AppStoreVersionRelationships from a dict
app_store_version_relationships_from_dict = AppStoreVersionRelationships.from_dict(app_store_version_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# BuildRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pre_release_version** | [**BuildRelationshipsPreReleaseVersion**](BuildRelationshipsPreReleaseVersion.md) |  | [optional] 
**individual_testers** | [**BetaGroupRelationshipsBetaTesters**](BetaGroupRelationshipsBetaTesters.md) |  | [optional] 
**beta_groups** | [**AppRelationshipsBetaGroups**](AppRelationshipsBetaGroups.md) |  | [optional] 
**beta_build_localizations** | [**BuildRelationshipsBetaBuildLocalizations**](BuildRelationshipsBetaBuildLocalizations.md) |  | [optional] 
**app_encryption_declaration** | [**BuildRelationshipsAppEncryptionDeclaration**](BuildRelationshipsAppEncryptionDeclaration.md) |  | [optional] 
**beta_app_review_submission** | [**BuildRelationshipsBetaAppReviewSubmission**](BuildRelationshipsBetaAppReviewSubmission.md) |  | [optional] 
**app** | [**BetaAppLocalizationRelationshipsApp**](BetaAppLocalizationRelationshipsApp.md) |  | [optional] 
**build_beta_detail** | [**BuildRelationshipsBuildBetaDetail**](BuildRelationshipsBuildBetaDetail.md) |  | [optional] 
**app_store_version** | [**AppClipDefaultExperienceRelationshipsReleaseWithAppStoreVersion**](AppClipDefaultExperienceRelationshipsReleaseWithAppStoreVersion.md) |  | [optional] 
**icons** | [**BuildRelationshipsIcons**](BuildRelationshipsIcons.md) |  | [optional] 
**build_bundles** | [**BuildRelationshipsBuildBundles**](BuildRelationshipsBuildBundles.md) |  | [optional] 
**perf_power_metrics** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**diagnostic_signatures** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.build_relationships import BuildRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of BuildRelationships from a JSON string
build_relationships_instance = BuildRelationships.from_json(json)
# print the JSON string representation of the object
print(BuildRelationships.to_json())

# convert the object into a dict
build_relationships_dict = build_relationships_instance.to_dict()
# create an instance of BuildRelationships from a dict
build_relationships_from_dict = BuildRelationships.from_dict(build_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



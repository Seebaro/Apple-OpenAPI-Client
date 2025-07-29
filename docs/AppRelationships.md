# AppRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accessibility_declarations** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**app_encryption_declarations** | [**AppRelationshipsAppEncryptionDeclarations**](AppRelationshipsAppEncryptionDeclarations.md) |  | [optional] 
**ci_product** | [**AppRelationshipsCiProduct**](AppRelationshipsCiProduct.md) |  | [optional] 
**beta_testers** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**beta_groups** | [**AppRelationshipsBetaGroups**](AppRelationshipsBetaGroups.md) |  | [optional] 
**app_store_versions** | [**AppRelationshipsAppStoreVersions**](AppRelationshipsAppStoreVersions.md) |  | [optional] 
**pre_release_versions** | [**AppRelationshipsPreReleaseVersions**](AppRelationshipsPreReleaseVersions.md) |  | [optional] 
**beta_app_localizations** | [**AppRelationshipsBetaAppLocalizations**](AppRelationshipsBetaAppLocalizations.md) |  | [optional] 
**builds** | [**AppRelationshipsBuilds**](AppRelationshipsBuilds.md) |  | [optional] 
**beta_license_agreement** | [**AppRelationshipsBetaLicenseAgreement**](AppRelationshipsBetaLicenseAgreement.md) |  | [optional] 
**beta_app_review_detail** | [**AppRelationshipsBetaAppReviewDetail**](AppRelationshipsBetaAppReviewDetail.md) |  | [optional] 
**app_infos** | [**AppRelationshipsAppInfos**](AppRelationshipsAppInfos.md) |  | [optional] 
**app_clips** | [**AppRelationshipsAppClips**](AppRelationshipsAppClips.md) |  | [optional] 
**app_price_points** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**end_user_license_agreement** | [**AppRelationshipsEndUserLicenseAgreement**](AppRelationshipsEndUserLicenseAgreement.md) |  | [optional] 
**app_price_schedule** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**app_availability_v2** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**in_app_purchases** | [**AppRelationshipsInAppPurchases**](AppRelationshipsInAppPurchases.md) |  | [optional] 
**subscription_groups** | [**AppRelationshipsSubscriptionGroups**](AppRelationshipsSubscriptionGroups.md) |  | [optional] 
**game_center_enabled_versions** | [**AppRelationshipsGameCenterEnabledVersions**](AppRelationshipsGameCenterEnabledVersions.md) |  | [optional] 
**perf_power_metrics** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**app_custom_product_pages** | [**AppRelationshipsAppCustomProductPages**](AppRelationshipsAppCustomProductPages.md) |  | [optional] 
**in_app_purchases_v2** | [**AppRelationshipsInAppPurchasesV2**](AppRelationshipsInAppPurchasesV2.md) |  | [optional] 
**promoted_purchases** | [**AppRelationshipsPromotedPurchases**](AppRelationshipsPromotedPurchases.md) |  | [optional] 
**app_events** | [**AppRelationshipsAppEvents**](AppRelationshipsAppEvents.md) |  | [optional] 
**review_submissions** | [**AppRelationshipsReviewSubmissions**](AppRelationshipsReviewSubmissions.md) |  | [optional] 
**subscription_grace_period** | [**AppRelationshipsSubscriptionGracePeriod**](AppRelationshipsSubscriptionGracePeriod.md) |  | [optional] 
**customer_reviews** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**customer_review_summarizations** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**game_center_detail** | [**AppRelationshipsGameCenterDetail**](AppRelationshipsGameCenterDetail.md) |  | [optional] 
**app_store_version_experiments_v2** | [**AppStoreVersionRelationshipsAppStoreVersionExperiments**](AppStoreVersionRelationshipsAppStoreVersionExperiments.md) |  | [optional] 
**alternative_distribution_key** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**analytics_report_requests** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**marketplace_search_detail** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**background_assets** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**beta_feedback_screenshot_submissions** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**beta_feedback_crash_submissions** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**webhooks** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_relationships import AppRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppRelationships from a JSON string
app_relationships_instance = AppRelationships.from_json(json)
# print the JSON string representation of the object
print(AppRelationships.to_json())

# convert the object into a dict
app_relationships_dict = app_relationships_instance.to_dict()
# create an instance of AppRelationships from a dict
app_relationships_from_dict = AppRelationships.from_dict(app_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



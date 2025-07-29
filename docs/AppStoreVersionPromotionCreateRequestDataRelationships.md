# AppStoreVersionPromotionCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_store_version** | [**AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersion**](AlternativeDistributionPackageCreateRequestDataRelationshipsAppStoreVersion.md) |  | 
**app_store_version_experiment_treatment** | [**AppStoreVersionExperimentTreatmentLocalizationCreateRequestDataRelationshipsAppStoreVersionExperimentTreatment**](AppStoreVersionExperimentTreatmentLocalizationCreateRequestDataRelationshipsAppStoreVersionExperimentTreatment.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_promotion_create_request_data_relationships import AppStoreVersionPromotionCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionPromotionCreateRequestDataRelationships from a JSON string
app_store_version_promotion_create_request_data_relationships_instance = AppStoreVersionPromotionCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionPromotionCreateRequestDataRelationships.to_json())

# convert the object into a dict
app_store_version_promotion_create_request_data_relationships_dict = app_store_version_promotion_create_request_data_relationships_instance.to_dict()
# create an instance of AppStoreVersionPromotionCreateRequestDataRelationships from a dict
app_store_version_promotion_create_request_data_relationships_from_dict = AppStoreVersionPromotionCreateRequestDataRelationships.from_dict(app_store_version_promotion_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



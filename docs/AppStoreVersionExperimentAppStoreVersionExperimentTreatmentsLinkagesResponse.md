# AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppStoreVersionExperimentTreatmentLocalizationRelationshipsAppStoreVersionExperimentTreatmentData]**](AppStoreVersionExperimentTreatmentLocalizationRelationshipsAppStoreVersionExperimentTreatmentData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiment_app_store_version_experiment_treatments_linkages_response import AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse from a JSON string
app_store_version_experiment_app_store_version_experiment_treatments_linkages_response_instance = AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse.to_json())

# convert the object into a dict
app_store_version_experiment_app_store_version_experiment_treatments_linkages_response_dict = app_store_version_experiment_app_store_version_experiment_treatments_linkages_response_instance.to_dict()
# create an instance of AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse from a dict
app_store_version_experiment_app_store_version_experiment_treatments_linkages_response_from_dict = AppStoreVersionExperimentAppStoreVersionExperimentTreatmentsLinkagesResponse.from_dict(app_store_version_experiment_app_store_version_experiment_treatments_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



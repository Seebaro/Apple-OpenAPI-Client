# AppStoreVersionExperimentsV2ResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AppStoreVersionExperimentTreatmentAttributes**](AppStoreVersionExperimentTreatmentAttributes.md) |  | [optional] 
**relationships** | [**AppStoreVersionExperimentTreatmentRelationships**](AppStoreVersionExperimentTreatmentRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.app_store_version_experiments_v2_response_included_inner import AppStoreVersionExperimentsV2ResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionExperimentsV2ResponseIncludedInner from a JSON string
app_store_version_experiments_v2_response_included_inner_instance = AppStoreVersionExperimentsV2ResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionExperimentsV2ResponseIncludedInner.to_json())

# convert the object into a dict
app_store_version_experiments_v2_response_included_inner_dict = app_store_version_experiments_v2_response_included_inner_instance.to_dict()
# create an instance of AppStoreVersionExperimentsV2ResponseIncludedInner from a dict
app_store_version_experiments_v2_response_included_inner_from_dict = AppStoreVersionExperimentsV2ResponseIncludedInner.from_dict(app_store_version_experiments_v2_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



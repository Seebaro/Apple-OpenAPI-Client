# CiProductRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**BetaAppLocalizationRelationshipsApp**](BetaAppLocalizationRelationshipsApp.md) |  | [optional] 
**bundle_id** | [**CiProductRelationshipsBundleId**](CiProductRelationshipsBundleId.md) |  | [optional] 
**workflows** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**primary_repositories** | [**CiProductRelationshipsPrimaryRepositories**](CiProductRelationshipsPrimaryRepositories.md) |  | [optional] 
**additional_repositories** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 
**build_runs** | [**AnalyticsReportInstanceRelationshipsSegments**](AnalyticsReportInstanceRelationshipsSegments.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_product_relationships import CiProductRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CiProductRelationships from a JSON string
ci_product_relationships_instance = CiProductRelationships.from_json(json)
# print the JSON string representation of the object
print(CiProductRelationships.to_json())

# convert the object into a dict
ci_product_relationships_dict = ci_product_relationships_instance.to_dict()
# create an instance of CiProductRelationships from a dict
ci_product_relationships_from_dict = CiProductRelationships.from_dict(ci_product_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



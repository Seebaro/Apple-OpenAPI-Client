# AppStoreVersionRoutingAppCoverageLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppStoreVersionRelationshipsRoutingAppCoverageData**](AppStoreVersionRelationshipsRoutingAppCoverageData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_routing_app_coverage_linkage_response import AppStoreVersionRoutingAppCoverageLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionRoutingAppCoverageLinkageResponse from a JSON string
app_store_version_routing_app_coverage_linkage_response_instance = AppStoreVersionRoutingAppCoverageLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionRoutingAppCoverageLinkageResponse.to_json())

# convert the object into a dict
app_store_version_routing_app_coverage_linkage_response_dict = app_store_version_routing_app_coverage_linkage_response_instance.to_dict()
# create an instance of AppStoreVersionRoutingAppCoverageLinkageResponse from a dict
app_store_version_routing_app_coverage_linkage_response_from_dict = AppStoreVersionRoutingAppCoverageLinkageResponse.from_dict(app_store_version_routing_app_coverage_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



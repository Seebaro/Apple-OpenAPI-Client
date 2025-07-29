# AppStoreVersionAlternativeDistributionPackageLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackageVersionRelationshipsAlternativeDistributionPackageData**](AlternativeDistributionPackageVersionRelationshipsAlternativeDistributionPackageData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_store_version_alternative_distribution_package_linkage_response import AppStoreVersionAlternativeDistributionPackageLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppStoreVersionAlternativeDistributionPackageLinkageResponse from a JSON string
app_store_version_alternative_distribution_package_linkage_response_instance = AppStoreVersionAlternativeDistributionPackageLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppStoreVersionAlternativeDistributionPackageLinkageResponse.to_json())

# convert the object into a dict
app_store_version_alternative_distribution_package_linkage_response_dict = app_store_version_alternative_distribution_package_linkage_response_instance.to_dict()
# create an instance of AppStoreVersionAlternativeDistributionPackageLinkageResponse from a dict
app_store_version_alternative_distribution_package_linkage_response_from_dict = AppStoreVersionAlternativeDistributionPackageLinkageResponse.from_dict(app_store_version_alternative_distribution_package_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AlternativeDistributionPackageVersionRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**variants** | [**AlternativeDistributionPackageVersionRelationshipsVariants**](AlternativeDistributionPackageVersionRelationshipsVariants.md) |  | [optional] 
**deltas** | [**AlternativeDistributionPackageVersionRelationshipsDeltas**](AlternativeDistributionPackageVersionRelationshipsDeltas.md) |  | [optional] 
**alternative_distribution_package** | [**AlternativeDistributionPackageVersionRelationshipsAlternativeDistributionPackage**](AlternativeDistributionPackageVersionRelationshipsAlternativeDistributionPackage.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_version_relationships import AlternativeDistributionPackageVersionRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersionRelationships from a JSON string
alternative_distribution_package_version_relationships_instance = AlternativeDistributionPackageVersionRelationships.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersionRelationships.to_json())

# convert the object into a dict
alternative_distribution_package_version_relationships_dict = alternative_distribution_package_version_relationships_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersionRelationships from a dict
alternative_distribution_package_version_relationships_from_dict = AlternativeDistributionPackageVersionRelationships.from_dict(alternative_distribution_package_version_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AlternativeDistributionPackageVersionRelationshipsVariants


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AlternativeDistributionPackageVersionRelationshipsVariantsDataInner]**](AlternativeDistributionPackageVersionRelationshipsVariantsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_version_relationships_variants import AlternativeDistributionPackageVersionRelationshipsVariants

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersionRelationshipsVariants from a JSON string
alternative_distribution_package_version_relationships_variants_instance = AlternativeDistributionPackageVersionRelationshipsVariants.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersionRelationshipsVariants.to_json())

# convert the object into a dict
alternative_distribution_package_version_relationships_variants_dict = alternative_distribution_package_version_relationships_variants_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersionRelationshipsVariants from a dict
alternative_distribution_package_version_relationships_variants_from_dict = AlternativeDistributionPackageVersionRelationshipsVariants.from_dict(alternative_distribution_package_version_relationships_variants_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AlternativeDistributionPackageRelationshipsVersions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AlternativeDistributionPackageRelationshipsVersionsDataInner]**](AlternativeDistributionPackageRelationshipsVersionsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_relationships_versions import AlternativeDistributionPackageRelationshipsVersions

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageRelationshipsVersions from a JSON string
alternative_distribution_package_relationships_versions_instance = AlternativeDistributionPackageRelationshipsVersions.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageRelationshipsVersions.to_json())

# convert the object into a dict
alternative_distribution_package_relationships_versions_dict = alternative_distribution_package_relationships_versions_instance.to_dict()
# create an instance of AlternativeDistributionPackageRelationshipsVersions from a dict
alternative_distribution_package_relationships_versions_from_dict = AlternativeDistributionPackageRelationshipsVersions.from_dict(alternative_distribution_package_relationships_versions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



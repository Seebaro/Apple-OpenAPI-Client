# AlternativeDistributionPackageVersionRelationshipsDeltas


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AlternativeDistributionPackageVersionRelationshipsDeltasDataInner]**](AlternativeDistributionPackageVersionRelationshipsDeltasDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_version_relationships_deltas import AlternativeDistributionPackageVersionRelationshipsDeltas

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersionRelationshipsDeltas from a JSON string
alternative_distribution_package_version_relationships_deltas_instance = AlternativeDistributionPackageVersionRelationshipsDeltas.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersionRelationshipsDeltas.to_json())

# convert the object into a dict
alternative_distribution_package_version_relationships_deltas_dict = alternative_distribution_package_version_relationships_deltas_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersionRelationshipsDeltas from a dict
alternative_distribution_package_version_relationships_deltas_from_dict = AlternativeDistributionPackageVersionRelationshipsDeltas.from_dict(alternative_distribution_package_version_relationships_deltas_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



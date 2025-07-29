# AlternativeDistributionPackageVersionsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AlternativeDistributionPackageDeltaAttributes**](AlternativeDistributionPackageDeltaAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 
**relationships** | [**AlternativeDistributionPackageRelationships**](AlternativeDistributionPackageRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_versions_response_included_inner import AlternativeDistributionPackageVersionsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersionsResponseIncludedInner from a JSON string
alternative_distribution_package_versions_response_included_inner_instance = AlternativeDistributionPackageVersionsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersionsResponseIncludedInner.to_json())

# convert the object into a dict
alternative_distribution_package_versions_response_included_inner_dict = alternative_distribution_package_versions_response_included_inner_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersionsResponseIncludedInner from a dict
alternative_distribution_package_versions_response_included_inner_from_dict = AlternativeDistributionPackageVersionsResponseIncludedInner.from_dict(alternative_distribution_package_versions_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



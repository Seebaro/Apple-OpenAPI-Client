# AlternativeDistributionPackageVersion


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AlternativeDistributionPackageVersionAttributes**](AlternativeDistributionPackageVersionAttributes.md) |  | [optional] 
**relationships** | [**AlternativeDistributionPackageVersionRelationships**](AlternativeDistributionPackageVersionRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_version import AlternativeDistributionPackageVersion

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersion from a JSON string
alternative_distribution_package_version_instance = AlternativeDistributionPackageVersion.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersion.to_json())

# convert the object into a dict
alternative_distribution_package_version_dict = alternative_distribution_package_version_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersion from a dict
alternative_distribution_package_version_from_dict = AlternativeDistributionPackageVersion.from_dict(alternative_distribution_package_version_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



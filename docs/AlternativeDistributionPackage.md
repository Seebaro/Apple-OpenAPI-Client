# AlternativeDistributionPackage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**relationships** | [**AlternativeDistributionPackageRelationships**](AlternativeDistributionPackageRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package import AlternativeDistributionPackage

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackage from a JSON string
alternative_distribution_package_instance = AlternativeDistributionPackage.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackage.to_json())

# convert the object into a dict
alternative_distribution_package_dict = alternative_distribution_package_instance.to_dict()
# create an instance of AlternativeDistributionPackage from a dict
alternative_distribution_package_from_dict = AlternativeDistributionPackage.from_dict(alternative_distribution_package_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



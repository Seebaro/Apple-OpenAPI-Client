# AlternativeDistributionPackageVariant


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AlternativeDistributionPackageDeltaAttributes**](AlternativeDistributionPackageDeltaAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_variant import AlternativeDistributionPackageVariant

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVariant from a JSON string
alternative_distribution_package_variant_instance = AlternativeDistributionPackageVariant.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVariant.to_json())

# convert the object into a dict
alternative_distribution_package_variant_dict = alternative_distribution_package_variant_instance.to_dict()
# create an instance of AlternativeDistributionPackageVariant from a dict
alternative_distribution_package_variant_from_dict = AlternativeDistributionPackageVariant.from_dict(alternative_distribution_package_variant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AlternativeDistributionPackageVariantResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackageVariant**](AlternativeDistributionPackageVariant.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_package_variant_response import AlternativeDistributionPackageVariantResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVariantResponse from a JSON string
alternative_distribution_package_variant_response_instance = AlternativeDistributionPackageVariantResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVariantResponse.to_json())

# convert the object into a dict
alternative_distribution_package_variant_response_dict = alternative_distribution_package_variant_response_instance.to_dict()
# create an instance of AlternativeDistributionPackageVariantResponse from a dict
alternative_distribution_package_variant_response_from_dict = AlternativeDistributionPackageVariantResponse.from_dict(alternative_distribution_package_variant_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



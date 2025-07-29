# AlternativeDistributionPackageVariantsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AlternativeDistributionPackageVariant]**](AlternativeDistributionPackageVariant.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_variants_response import AlternativeDistributionPackageVariantsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVariantsResponse from a JSON string
alternative_distribution_package_variants_response_instance = AlternativeDistributionPackageVariantsResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVariantsResponse.to_json())

# convert the object into a dict
alternative_distribution_package_variants_response_dict = alternative_distribution_package_variants_response_instance.to_dict()
# create an instance of AlternativeDistributionPackageVariantsResponse from a dict
alternative_distribution_package_variants_response_from_dict = AlternativeDistributionPackageVariantsResponse.from_dict(alternative_distribution_package_variants_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



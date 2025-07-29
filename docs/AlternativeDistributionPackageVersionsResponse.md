# AlternativeDistributionPackageVersionsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AlternativeDistributionPackageVersion]**](AlternativeDistributionPackageVersion.md) |  | 
**included** | [**List[AlternativeDistributionPackageVersionsResponseIncludedInner]**](AlternativeDistributionPackageVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_versions_response import AlternativeDistributionPackageVersionsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersionsResponse from a JSON string
alternative_distribution_package_versions_response_instance = AlternativeDistributionPackageVersionsResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersionsResponse.to_json())

# convert the object into a dict
alternative_distribution_package_versions_response_dict = alternative_distribution_package_versions_response_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersionsResponse from a dict
alternative_distribution_package_versions_response_from_dict = AlternativeDistributionPackageVersionsResponse.from_dict(alternative_distribution_package_versions_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



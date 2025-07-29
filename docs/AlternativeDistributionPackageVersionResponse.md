# AlternativeDistributionPackageVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackageVersion**](AlternativeDistributionPackageVersion.md) |  | 
**included** | [**List[AlternativeDistributionPackageVersionsResponseIncludedInner]**](AlternativeDistributionPackageVersionsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_package_version_response import AlternativeDistributionPackageVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersionResponse from a JSON string
alternative_distribution_package_version_response_instance = AlternativeDistributionPackageVersionResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersionResponse.to_json())

# convert the object into a dict
alternative_distribution_package_version_response_dict = alternative_distribution_package_version_response_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersionResponse from a dict
alternative_distribution_package_version_response_from_dict = AlternativeDistributionPackageVersionResponse.from_dict(alternative_distribution_package_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



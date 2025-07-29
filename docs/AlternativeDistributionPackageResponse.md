# AlternativeDistributionPackageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackage**](AlternativeDistributionPackage.md) |  | 
**included** | [**List[AlternativeDistributionPackageVersion]**](AlternativeDistributionPackageVersion.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_package_response import AlternativeDistributionPackageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageResponse from a JSON string
alternative_distribution_package_response_instance = AlternativeDistributionPackageResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageResponse.to_json())

# convert the object into a dict
alternative_distribution_package_response_dict = alternative_distribution_package_response_instance.to_dict()
# create an instance of AlternativeDistributionPackageResponse from a dict
alternative_distribution_package_response_from_dict = AlternativeDistributionPackageResponse.from_dict(alternative_distribution_package_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



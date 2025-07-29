# AlternativeDistributionPackageDeltaResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackageDelta**](AlternativeDistributionPackageDelta.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_package_delta_response import AlternativeDistributionPackageDeltaResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageDeltaResponse from a JSON string
alternative_distribution_package_delta_response_instance = AlternativeDistributionPackageDeltaResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageDeltaResponse.to_json())

# convert the object into a dict
alternative_distribution_package_delta_response_dict = alternative_distribution_package_delta_response_instance.to_dict()
# create an instance of AlternativeDistributionPackageDeltaResponse from a dict
alternative_distribution_package_delta_response_from_dict = AlternativeDistributionPackageDeltaResponse.from_dict(alternative_distribution_package_delta_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



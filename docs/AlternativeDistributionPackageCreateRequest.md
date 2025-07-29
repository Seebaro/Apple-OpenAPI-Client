# AlternativeDistributionPackageCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionPackageCreateRequestData**](AlternativeDistributionPackageCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_package_create_request import AlternativeDistributionPackageCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageCreateRequest from a JSON string
alternative_distribution_package_create_request_instance = AlternativeDistributionPackageCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageCreateRequest.to_json())

# convert the object into a dict
alternative_distribution_package_create_request_dict = alternative_distribution_package_create_request_instance.to_dict()
# create an instance of AlternativeDistributionPackageCreateRequest from a dict
alternative_distribution_package_create_request_from_dict = AlternativeDistributionPackageCreateRequest.from_dict(alternative_distribution_package_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



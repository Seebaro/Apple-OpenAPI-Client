# AlternativeDistributionPackageCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**AlternativeDistributionPackageCreateRequestDataRelationships**](AlternativeDistributionPackageCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_package_create_request_data import AlternativeDistributionPackageCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageCreateRequestData from a JSON string
alternative_distribution_package_create_request_data_instance = AlternativeDistributionPackageCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageCreateRequestData.to_json())

# convert the object into a dict
alternative_distribution_package_create_request_data_dict = alternative_distribution_package_create_request_data_instance.to_dict()
# create an instance of AlternativeDistributionPackageCreateRequestData from a dict
alternative_distribution_package_create_request_data_from_dict = AlternativeDistributionPackageCreateRequestData.from_dict(alternative_distribution_package_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



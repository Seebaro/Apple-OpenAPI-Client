# AlternativeDistributionPackageVersionAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | [optional] 
**url_expiration_date** | **datetime** |  | [optional] 
**version** | **str** |  | [optional] 
**file_checksum** | **str** |  | [optional] 
**state** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_version_attributes import AlternativeDistributionPackageVersionAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageVersionAttributes from a JSON string
alternative_distribution_package_version_attributes_instance = AlternativeDistributionPackageVersionAttributes.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageVersionAttributes.to_json())

# convert the object into a dict
alternative_distribution_package_version_attributes_dict = alternative_distribution_package_version_attributes_instance.to_dict()
# create an instance of AlternativeDistributionPackageVersionAttributes from a dict
alternative_distribution_package_version_attributes_from_dict = AlternativeDistributionPackageVersionAttributes.from_dict(alternative_distribution_package_version_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AlternativeDistributionPackageDeltaAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | [optional] 
**url_expiration_date** | **datetime** |  | [optional] 
**alternative_distribution_key_blob** | **str** |  | [optional] 
**file_checksum** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_delta_attributes import AlternativeDistributionPackageDeltaAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageDeltaAttributes from a JSON string
alternative_distribution_package_delta_attributes_instance = AlternativeDistributionPackageDeltaAttributes.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageDeltaAttributes.to_json())

# convert the object into a dict
alternative_distribution_package_delta_attributes_dict = alternative_distribution_package_delta_attributes_instance.to_dict()
# create an instance of AlternativeDistributionPackageDeltaAttributes from a dict
alternative_distribution_package_delta_attributes_from_dict = AlternativeDistributionPackageDeltaAttributes.from_dict(alternative_distribution_package_delta_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



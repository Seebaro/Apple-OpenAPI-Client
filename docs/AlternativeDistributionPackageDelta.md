# AlternativeDistributionPackageDelta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AlternativeDistributionPackageDeltaAttributes**](AlternativeDistributionPackageDeltaAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_delta import AlternativeDistributionPackageDelta

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageDelta from a JSON string
alternative_distribution_package_delta_instance = AlternativeDistributionPackageDelta.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageDelta.to_json())

# convert the object into a dict
alternative_distribution_package_delta_dict = alternative_distribution_package_delta_instance.to_dict()
# create an instance of AlternativeDistributionPackageDelta from a dict
alternative_distribution_package_delta_from_dict = AlternativeDistributionPackageDelta.from_dict(alternative_distribution_package_delta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



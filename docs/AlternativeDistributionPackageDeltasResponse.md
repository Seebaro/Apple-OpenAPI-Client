# AlternativeDistributionPackageDeltasResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AlternativeDistributionPackageDelta]**](AlternativeDistributionPackageDelta.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_package_deltas_response import AlternativeDistributionPackageDeltasResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionPackageDeltasResponse from a JSON string
alternative_distribution_package_deltas_response_instance = AlternativeDistributionPackageDeltasResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionPackageDeltasResponse.to_json())

# convert the object into a dict
alternative_distribution_package_deltas_response_dict = alternative_distribution_package_deltas_response_instance.to_dict()
# create an instance of AlternativeDistributionPackageDeltasResponse from a dict
alternative_distribution_package_deltas_response_from_dict = AlternativeDistributionPackageDeltasResponse.from_dict(alternative_distribution_package_deltas_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



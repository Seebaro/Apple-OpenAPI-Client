# AlternativeDistributionKeysResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AlternativeDistributionKey]**](AlternativeDistributionKey.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_keys_response import AlternativeDistributionKeysResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionKeysResponse from a JSON string
alternative_distribution_keys_response_instance = AlternativeDistributionKeysResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionKeysResponse.to_json())

# convert the object into a dict
alternative_distribution_keys_response_dict = alternative_distribution_keys_response_instance.to_dict()
# create an instance of AlternativeDistributionKeysResponse from a dict
alternative_distribution_keys_response_from_dict = AlternativeDistributionKeysResponse.from_dict(alternative_distribution_keys_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



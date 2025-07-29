# AlternativeDistributionKeyResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionKey**](AlternativeDistributionKey.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_key_response import AlternativeDistributionKeyResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionKeyResponse from a JSON string
alternative_distribution_key_response_instance = AlternativeDistributionKeyResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionKeyResponse.to_json())

# convert the object into a dict
alternative_distribution_key_response_dict = alternative_distribution_key_response_instance.to_dict()
# create an instance of AlternativeDistributionKeyResponse from a dict
alternative_distribution_key_response_from_dict = AlternativeDistributionKeyResponse.from_dict(alternative_distribution_key_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



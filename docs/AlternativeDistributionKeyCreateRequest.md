# AlternativeDistributionKeyCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionKeyCreateRequestData**](AlternativeDistributionKeyCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_key_create_request import AlternativeDistributionKeyCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionKeyCreateRequest from a JSON string
alternative_distribution_key_create_request_instance = AlternativeDistributionKeyCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionKeyCreateRequest.to_json())

# convert the object into a dict
alternative_distribution_key_create_request_dict = alternative_distribution_key_create_request_instance.to_dict()
# create an instance of AlternativeDistributionKeyCreateRequest from a dict
alternative_distribution_key_create_request_from_dict = AlternativeDistributionKeyCreateRequest.from_dict(alternative_distribution_key_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AlternativeDistributionDomainCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionDomainCreateRequestData**](AlternativeDistributionDomainCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_domain_create_request import AlternativeDistributionDomainCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionDomainCreateRequest from a JSON string
alternative_distribution_domain_create_request_instance = AlternativeDistributionDomainCreateRequest.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionDomainCreateRequest.to_json())

# convert the object into a dict
alternative_distribution_domain_create_request_dict = alternative_distribution_domain_create_request_instance.to_dict()
# create an instance of AlternativeDistributionDomainCreateRequest from a dict
alternative_distribution_domain_create_request_from_dict = AlternativeDistributionDomainCreateRequest.from_dict(alternative_distribution_domain_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



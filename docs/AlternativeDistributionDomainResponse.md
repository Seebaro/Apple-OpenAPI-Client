# AlternativeDistributionDomainResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AlternativeDistributionDomain**](AlternativeDistributionDomain.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_domain_response import AlternativeDistributionDomainResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionDomainResponse from a JSON string
alternative_distribution_domain_response_instance = AlternativeDistributionDomainResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionDomainResponse.to_json())

# convert the object into a dict
alternative_distribution_domain_response_dict = alternative_distribution_domain_response_instance.to_dict()
# create an instance of AlternativeDistributionDomainResponse from a dict
alternative_distribution_domain_response_from_dict = AlternativeDistributionDomainResponse.from_dict(alternative_distribution_domain_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



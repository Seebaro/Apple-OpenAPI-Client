# AlternativeDistributionDomainsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AlternativeDistributionDomain]**](AlternativeDistributionDomain.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_domains_response import AlternativeDistributionDomainsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionDomainsResponse from a JSON string
alternative_distribution_domains_response_instance = AlternativeDistributionDomainsResponse.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionDomainsResponse.to_json())

# convert the object into a dict
alternative_distribution_domains_response_dict = alternative_distribution_domains_response_instance.to_dict()
# create an instance of AlternativeDistributionDomainsResponse from a dict
alternative_distribution_domains_response_from_dict = AlternativeDistributionDomainsResponse.from_dict(alternative_distribution_domains_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



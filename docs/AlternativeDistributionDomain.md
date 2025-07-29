# AlternativeDistributionDomain


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AlternativeDistributionDomainAttributes**](AlternativeDistributionDomainAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_domain import AlternativeDistributionDomain

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionDomain from a JSON string
alternative_distribution_domain_instance = AlternativeDistributionDomain.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionDomain.to_json())

# convert the object into a dict
alternative_distribution_domain_dict = alternative_distribution_domain_instance.to_dict()
# create an instance of AlternativeDistributionDomain from a dict
alternative_distribution_domain_from_dict = AlternativeDistributionDomain.from_dict(alternative_distribution_domain_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



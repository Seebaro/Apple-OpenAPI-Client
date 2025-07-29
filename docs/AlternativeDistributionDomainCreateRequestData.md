# AlternativeDistributionDomainCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AlternativeDistributionDomainCreateRequestDataAttributes**](AlternativeDistributionDomainCreateRequestDataAttributes.md) |  | 

## Example

```python
from openapi_client.models.alternative_distribution_domain_create_request_data import AlternativeDistributionDomainCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionDomainCreateRequestData from a JSON string
alternative_distribution_domain_create_request_data_instance = AlternativeDistributionDomainCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionDomainCreateRequestData.to_json())

# convert the object into a dict
alternative_distribution_domain_create_request_data_dict = alternative_distribution_domain_create_request_data_instance.to_dict()
# create an instance of AlternativeDistributionDomainCreateRequestData from a dict
alternative_distribution_domain_create_request_data_from_dict = AlternativeDistributionDomainCreateRequestData.from_dict(alternative_distribution_domain_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



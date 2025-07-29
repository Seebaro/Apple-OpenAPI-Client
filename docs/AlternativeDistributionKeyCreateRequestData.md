# AlternativeDistributionKeyCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**AlternativeDistributionKeyCreateRequestDataAttributes**](AlternativeDistributionKeyCreateRequestDataAttributes.md) |  | 
**relationships** | [**AlternativeDistributionKeyCreateRequestDataRelationships**](AlternativeDistributionKeyCreateRequestDataRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_key_create_request_data import AlternativeDistributionKeyCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionKeyCreateRequestData from a JSON string
alternative_distribution_key_create_request_data_instance = AlternativeDistributionKeyCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionKeyCreateRequestData.to_json())

# convert the object into a dict
alternative_distribution_key_create_request_data_dict = alternative_distribution_key_create_request_data_instance.to_dict()
# create an instance of AlternativeDistributionKeyCreateRequestData from a dict
alternative_distribution_key_create_request_data_from_dict = AlternativeDistributionKeyCreateRequestData.from_dict(alternative_distribution_key_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



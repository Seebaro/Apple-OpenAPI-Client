# AlternativeDistributionKey


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**AlternativeDistributionKeyAttributes**](AlternativeDistributionKeyAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.alternative_distribution_key import AlternativeDistributionKey

# TODO update the JSON string below
json = "{}"
# create an instance of AlternativeDistributionKey from a JSON string
alternative_distribution_key_instance = AlternativeDistributionKey.from_json(json)
# print the JSON string representation of the object
print(AlternativeDistributionKey.to_json())

# convert the object into a dict
alternative_distribution_key_dict = alternative_distribution_key_instance.to_dict()
# create an instance of AlternativeDistributionKey from a dict
alternative_distribution_key_from_dict = AlternativeDistributionKey.from_dict(alternative_distribution_key_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



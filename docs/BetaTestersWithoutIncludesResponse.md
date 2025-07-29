# BetaTestersWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BetaTester]**](BetaTester.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_testers_without_includes_response import BetaTestersWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaTestersWithoutIncludesResponse from a JSON string
beta_testers_without_includes_response_instance = BetaTestersWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(BetaTestersWithoutIncludesResponse.to_json())

# convert the object into a dict
beta_testers_without_includes_response_dict = beta_testers_without_includes_response_instance.to_dict()
# create an instance of BetaTestersWithoutIncludesResponse from a dict
beta_testers_without_includes_response_from_dict = BetaTestersWithoutIncludesResponse.from_dict(beta_testers_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



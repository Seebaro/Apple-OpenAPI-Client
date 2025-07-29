# NominationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**Nomination**](Nomination.md) |  | 
**included** | [**List[NominationsResponseIncludedInner]**](NominationsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.nomination_response import NominationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of NominationResponse from a JSON string
nomination_response_instance = NominationResponse.from_json(json)
# print the JSON string representation of the object
print(NominationResponse.to_json())

# convert the object into a dict
nomination_response_dict = nomination_response_instance.to_dict()
# create an instance of NominationResponse from a dict
nomination_response_from_dict = NominationResponse.from_dict(nomination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



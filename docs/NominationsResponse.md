# NominationsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Nomination]**](Nomination.md) |  | 
**included** | [**List[NominationsResponseIncludedInner]**](NominationsResponseIncludedInner.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.nominations_response import NominationsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of NominationsResponse from a JSON string
nominations_response_instance = NominationsResponse.from_json(json)
# print the JSON string representation of the object
print(NominationsResponse.to_json())

# convert the object into a dict
nominations_response_dict = nominations_response_instance.to_dict()
# create an instance of NominationsResponse from a dict
nominations_response_from_dict = NominationsResponse.from_dict(nominations_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



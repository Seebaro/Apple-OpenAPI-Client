# CertificatesWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Certificate]**](Certificate.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.certificates_without_includes_response import CertificatesWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CertificatesWithoutIncludesResponse from a JSON string
certificates_without_includes_response_instance = CertificatesWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(CertificatesWithoutIncludesResponse.to_json())

# convert the object into a dict
certificates_without_includes_response_dict = certificates_without_includes_response_instance.to_dict()
# create an instance of CertificatesWithoutIncludesResponse from a dict
certificates_without_includes_response_from_dict = CertificatesWithoutIncludesResponse.from_dict(certificates_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



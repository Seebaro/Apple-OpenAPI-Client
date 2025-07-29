# PassTypeIdCertificatesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[MerchantIdRelationshipsCertificatesDataInner]**](MerchantIdRelationshipsCertificatesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.pass_type_id_certificates_linkages_response import PassTypeIdCertificatesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PassTypeIdCertificatesLinkagesResponse from a JSON string
pass_type_id_certificates_linkages_response_instance = PassTypeIdCertificatesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(PassTypeIdCertificatesLinkagesResponse.to_json())

# convert the object into a dict
pass_type_id_certificates_linkages_response_dict = pass_type_id_certificates_linkages_response_instance.to_dict()
# create an instance of PassTypeIdCertificatesLinkagesResponse from a dict
pass_type_id_certificates_linkages_response_from_dict = PassTypeIdCertificatesLinkagesResponse.from_dict(pass_type_id_certificates_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



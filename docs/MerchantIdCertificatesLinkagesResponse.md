# MerchantIdCertificatesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[MerchantIdRelationshipsCertificatesDataInner]**](MerchantIdRelationshipsCertificatesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.merchant_id_certificates_linkages_response import MerchantIdCertificatesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdCertificatesLinkagesResponse from a JSON string
merchant_id_certificates_linkages_response_instance = MerchantIdCertificatesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(MerchantIdCertificatesLinkagesResponse.to_json())

# convert the object into a dict
merchant_id_certificates_linkages_response_dict = merchant_id_certificates_linkages_response_instance.to_dict()
# create an instance of MerchantIdCertificatesLinkagesResponse from a dict
merchant_id_certificates_linkages_response_from_dict = MerchantIdCertificatesLinkagesResponse.from_dict(merchant_id_certificates_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



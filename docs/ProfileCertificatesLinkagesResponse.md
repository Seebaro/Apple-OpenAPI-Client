# ProfileCertificatesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[MerchantIdRelationshipsCertificatesDataInner]**](MerchantIdRelationshipsCertificatesDataInner.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.profile_certificates_linkages_response import ProfileCertificatesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ProfileCertificatesLinkagesResponse from a JSON string
profile_certificates_linkages_response_instance = ProfileCertificatesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(ProfileCertificatesLinkagesResponse.to_json())

# convert the object into a dict
profile_certificates_linkages_response_dict = profile_certificates_linkages_response_instance.to_dict()
# create an instance of ProfileCertificatesLinkagesResponse from a dict
profile_certificates_linkages_response_from_dict = ProfileCertificatesLinkagesResponse.from_dict(profile_certificates_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



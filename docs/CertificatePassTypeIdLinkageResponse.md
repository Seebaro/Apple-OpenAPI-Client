# CertificatePassTypeIdLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CertificateRelationshipsPassTypeIdData**](CertificateRelationshipsPassTypeIdData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.certificate_pass_type_id_linkage_response import CertificatePassTypeIdLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CertificatePassTypeIdLinkageResponse from a JSON string
certificate_pass_type_id_linkage_response_instance = CertificatePassTypeIdLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(CertificatePassTypeIdLinkageResponse.to_json())

# convert the object into a dict
certificate_pass_type_id_linkage_response_dict = certificate_pass_type_id_linkage_response_instance.to_dict()
# create an instance of CertificatePassTypeIdLinkageResponse from a dict
certificate_pass_type_id_linkage_response_from_dict = CertificatePassTypeIdLinkageResponse.from_dict(certificate_pass_type_id_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



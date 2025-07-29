# CertificateCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**merchant_id** | [**CertificateCreateRequestDataRelationshipsMerchantId**](CertificateCreateRequestDataRelationshipsMerchantId.md) |  | [optional] 
**pass_type_id** | [**CertificateCreateRequestDataRelationshipsPassTypeId**](CertificateCreateRequestDataRelationshipsPassTypeId.md) |  | [optional] 

## Example

```python
from openapi_client.models.certificate_create_request_data_relationships import CertificateCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateCreateRequestDataRelationships from a JSON string
certificate_create_request_data_relationships_instance = CertificateCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(CertificateCreateRequestDataRelationships.to_json())

# convert the object into a dict
certificate_create_request_data_relationships_dict = certificate_create_request_data_relationships_instance.to_dict()
# create an instance of CertificateCreateRequestDataRelationships from a dict
certificate_create_request_data_relationships_from_dict = CertificateCreateRequestDataRelationships.from_dict(certificate_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



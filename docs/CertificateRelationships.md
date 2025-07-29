# CertificateRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pass_type_id** | [**CertificateRelationshipsPassTypeId**](CertificateRelationshipsPassTypeId.md) |  | [optional] 

## Example

```python
from openapi_client.models.certificate_relationships import CertificateRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateRelationships from a JSON string
certificate_relationships_instance = CertificateRelationships.from_json(json)
# print the JSON string representation of the object
print(CertificateRelationships.to_json())

# convert the object into a dict
certificate_relationships_dict = certificate_relationships_instance.to_dict()
# create an instance of CertificateRelationships from a dict
certificate_relationships_from_dict = CertificateRelationships.from_dict(certificate_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



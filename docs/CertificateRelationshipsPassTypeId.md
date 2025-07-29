# CertificateRelationshipsPassTypeId


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**CertificateRelationshipsPassTypeIdData**](CertificateRelationshipsPassTypeIdData.md) |  | [optional] 

## Example

```python
from openapi_client.models.certificate_relationships_pass_type_id import CertificateRelationshipsPassTypeId

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateRelationshipsPassTypeId from a JSON string
certificate_relationships_pass_type_id_instance = CertificateRelationshipsPassTypeId.from_json(json)
# print the JSON string representation of the object
print(CertificateRelationshipsPassTypeId.to_json())

# convert the object into a dict
certificate_relationships_pass_type_id_dict = certificate_relationships_pass_type_id_instance.to_dict()
# create an instance of CertificateRelationshipsPassTypeId from a dict
certificate_relationships_pass_type_id_from_dict = CertificateRelationshipsPassTypeId.from_dict(certificate_relationships_pass_type_id_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



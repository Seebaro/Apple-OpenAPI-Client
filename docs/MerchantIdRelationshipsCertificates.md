# MerchantIdRelationshipsCertificates


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[MerchantIdRelationshipsCertificatesDataInner]**](MerchantIdRelationshipsCertificatesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.merchant_id_relationships_certificates import MerchantIdRelationshipsCertificates

# TODO update the JSON string below
json = "{}"
# create an instance of MerchantIdRelationshipsCertificates from a JSON string
merchant_id_relationships_certificates_instance = MerchantIdRelationshipsCertificates.from_json(json)
# print the JSON string representation of the object
print(MerchantIdRelationshipsCertificates.to_json())

# convert the object into a dict
merchant_id_relationships_certificates_dict = merchant_id_relationships_certificates_instance.to_dict()
# create an instance of MerchantIdRelationshipsCertificates from a dict
merchant_id_relationships_certificates_from_dict = MerchantIdRelationshipsCertificates.from_dict(merchant_id_relationships_certificates_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



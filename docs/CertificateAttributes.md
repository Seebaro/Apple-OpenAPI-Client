# CertificateAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**certificate_type** | [**CertificateType**](CertificateType.md) |  | [optional] 
**display_name** | **str** |  | [optional] 
**serial_number** | **str** |  | [optional] 
**platform** | [**BundleIdPlatform**](BundleIdPlatform.md) |  | [optional] 
**expiration_date** | **datetime** |  | [optional] 
**certificate_content** | **str** |  | [optional] 
**activated** | **bool** |  | [optional] 

## Example

```python
from openapi_client.models.certificate_attributes import CertificateAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateAttributes from a JSON string
certificate_attributes_instance = CertificateAttributes.from_json(json)
# print the JSON string representation of the object
print(CertificateAttributes.to_json())

# convert the object into a dict
certificate_attributes_dict = certificate_attributes_instance.to_dict()
# create an instance of CertificateAttributes from a dict
certificate_attributes_from_dict = CertificateAttributes.from_dict(certificate_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



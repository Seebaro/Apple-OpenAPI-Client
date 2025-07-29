# CertificateUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CertificateUpdateRequestDataAttributes**](CertificateUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.certificate_update_request_data import CertificateUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateUpdateRequestData from a JSON string
certificate_update_request_data_instance = CertificateUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(CertificateUpdateRequestData.to_json())

# convert the object into a dict
certificate_update_request_data_dict = certificate_update_request_data_instance.to_dict()
# create an instance of CertificateUpdateRequestData from a dict
certificate_update_request_data_from_dict = CertificateUpdateRequestData.from_dict(certificate_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



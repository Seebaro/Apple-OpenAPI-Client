# CertificateUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CertificateUpdateRequestData**](CertificateUpdateRequestData.md) |  | 

## Example

```python
from openapi_client.models.certificate_update_request import CertificateUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateUpdateRequest from a JSON string
certificate_update_request_instance = CertificateUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CertificateUpdateRequest.to_json())

# convert the object into a dict
certificate_update_request_dict = certificate_update_request_instance.to_dict()
# create an instance of CertificateUpdateRequest from a dict
certificate_update_request_from_dict = CertificateUpdateRequest.from_dict(certificate_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



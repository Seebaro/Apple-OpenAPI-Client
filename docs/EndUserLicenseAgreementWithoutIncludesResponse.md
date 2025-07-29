# EndUserLicenseAgreementWithoutIncludesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**EndUserLicenseAgreement**](EndUserLicenseAgreement.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.end_user_license_agreement_without_includes_response import EndUserLicenseAgreementWithoutIncludesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EndUserLicenseAgreementWithoutIncludesResponse from a JSON string
end_user_license_agreement_without_includes_response_instance = EndUserLicenseAgreementWithoutIncludesResponse.from_json(json)
# print the JSON string representation of the object
print(EndUserLicenseAgreementWithoutIncludesResponse.to_json())

# convert the object into a dict
end_user_license_agreement_without_includes_response_dict = end_user_license_agreement_without_includes_response_instance.to_dict()
# create an instance of EndUserLicenseAgreementWithoutIncludesResponse from a dict
end_user_license_agreement_without_includes_response_from_dict = EndUserLicenseAgreementWithoutIncludesResponse.from_dict(end_user_license_agreement_without_includes_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



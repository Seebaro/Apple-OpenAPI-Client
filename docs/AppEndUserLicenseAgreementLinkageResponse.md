# AppEndUserLicenseAgreementLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsEndUserLicenseAgreementData**](AppRelationshipsEndUserLicenseAgreementData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_end_user_license_agreement_linkage_response import AppEndUserLicenseAgreementLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppEndUserLicenseAgreementLinkageResponse from a JSON string
app_end_user_license_agreement_linkage_response_instance = AppEndUserLicenseAgreementLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppEndUserLicenseAgreementLinkageResponse.to_json())

# convert the object into a dict
app_end_user_license_agreement_linkage_response_dict = app_end_user_license_agreement_linkage_response_instance.to_dict()
# create an instance of AppEndUserLicenseAgreementLinkageResponse from a dict
app_end_user_license_agreement_linkage_response_from_dict = AppEndUserLicenseAgreementLinkageResponse.from_dict(app_end_user_license_agreement_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



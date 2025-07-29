# AppBetaLicenseAgreementLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsBetaLicenseAgreementData**](AppRelationshipsBetaLicenseAgreementData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_beta_license_agreement_linkage_response import AppBetaLicenseAgreementLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppBetaLicenseAgreementLinkageResponse from a JSON string
app_beta_license_agreement_linkage_response_instance = AppBetaLicenseAgreementLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppBetaLicenseAgreementLinkageResponse.to_json())

# convert the object into a dict
app_beta_license_agreement_linkage_response_dict = app_beta_license_agreement_linkage_response_instance.to_dict()
# create an instance of AppBetaLicenseAgreementLinkageResponse from a dict
app_beta_license_agreement_linkage_response_from_dict = AppBetaLicenseAgreementLinkageResponse.from_dict(app_beta_license_agreement_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



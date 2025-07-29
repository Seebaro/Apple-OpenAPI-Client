# EndUserLicenseAgreementTerritoriesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPricePointV3RelationshipsTerritoryData]**](AppPricePointV3RelationshipsTerritoryData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.end_user_license_agreement_territories_linkages_response import EndUserLicenseAgreementTerritoriesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EndUserLicenseAgreementTerritoriesLinkagesResponse from a JSON string
end_user_license_agreement_territories_linkages_response_instance = EndUserLicenseAgreementTerritoriesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(EndUserLicenseAgreementTerritoriesLinkagesResponse.to_json())

# convert the object into a dict
end_user_license_agreement_territories_linkages_response_dict = end_user_license_agreement_territories_linkages_response_instance.to_dict()
# create an instance of EndUserLicenseAgreementTerritoriesLinkagesResponse from a dict
end_user_license_agreement_territories_linkages_response_from_dict = EndUserLicenseAgreementTerritoriesLinkagesResponse.from_dict(end_user_license_agreement_territories_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



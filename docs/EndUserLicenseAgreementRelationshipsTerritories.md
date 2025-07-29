# EndUserLicenseAgreementRelationshipsTerritories


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[AppPricePointV3RelationshipsTerritoryData]**](AppPricePointV3RelationshipsTerritoryData.md) |  | [optional] 

## Example

```python
from openapi_client.models.end_user_license_agreement_relationships_territories import EndUserLicenseAgreementRelationshipsTerritories

# TODO update the JSON string below
json = "{}"
# create an instance of EndUserLicenseAgreementRelationshipsTerritories from a JSON string
end_user_license_agreement_relationships_territories_instance = EndUserLicenseAgreementRelationshipsTerritories.from_json(json)
# print the JSON string representation of the object
print(EndUserLicenseAgreementRelationshipsTerritories.to_json())

# convert the object into a dict
end_user_license_agreement_relationships_territories_dict = end_user_license_agreement_relationships_territories_instance.to_dict()
# create an instance of EndUserLicenseAgreementRelationshipsTerritories from a dict
end_user_license_agreement_relationships_territories_from_dict = EndUserLicenseAgreementRelationshipsTerritories.from_dict(end_user_license_agreement_relationships_territories_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



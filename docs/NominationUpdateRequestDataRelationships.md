# NominationUpdateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**related_apps** | [**NominationUpdateRequestDataRelationshipsRelatedApps**](NominationUpdateRequestDataRelationshipsRelatedApps.md) |  | [optional] 
**in_app_events** | [**NominationCreateRequestDataRelationshipsInAppEvents**](NominationCreateRequestDataRelationshipsInAppEvents.md) |  | [optional] 
**supported_territories** | [**EndUserLicenseAgreementUpdateRequestDataRelationshipsTerritories**](EndUserLicenseAgreementUpdateRequestDataRelationshipsTerritories.md) |  | [optional] 

## Example

```python
from openapi_client.models.nomination_update_request_data_relationships import NominationUpdateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of NominationUpdateRequestDataRelationships from a JSON string
nomination_update_request_data_relationships_instance = NominationUpdateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(NominationUpdateRequestDataRelationships.to_json())

# convert the object into a dict
nomination_update_request_data_relationships_dict = nomination_update_request_data_relationships_instance.to_dict()
# create an instance of NominationUpdateRequestDataRelationships from a dict
nomination_update_request_data_relationships_from_dict = NominationUpdateRequestDataRelationships.from_dict(nomination_update_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



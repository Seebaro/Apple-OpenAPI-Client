# InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPricePointV3RelationshipsTerritoryData]**](AppPricePointV3RelationshipsTerritoryData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_availability_available_territories_linkages_response import InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse from a JSON string
in_app_purchase_availability_available_territories_linkages_response_instance = InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse.to_json())

# convert the object into a dict
in_app_purchase_availability_available_territories_linkages_response_dict = in_app_purchase_availability_available_territories_linkages_response_instance.to_dict()
# create an instance of InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse from a dict
in_app_purchase_availability_available_territories_linkages_response_from_dict = InAppPurchaseAvailabilityAvailableTerritoriesLinkagesResponse.from_dict(in_app_purchase_availability_available_territories_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



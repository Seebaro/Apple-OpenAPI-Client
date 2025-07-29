# SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AppPricePointV3RelationshipsTerritoryData]**](AppPricePointV3RelationshipsTerritoryData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.subscription_availability_available_territories_linkages_response import SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse from a JSON string
subscription_availability_available_territories_linkages_response_instance = SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse.to_json())

# convert the object into a dict
subscription_availability_available_territories_linkages_response_dict = subscription_availability_available_territories_linkages_response_instance.to_dict()
# create an instance of SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse from a dict
subscription_availability_available_territories_linkages_response_from_dict = SubscriptionAvailabilityAvailableTerritoriesLinkagesResponse.from_dict(subscription_availability_available_territories_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



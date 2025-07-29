# InAppPurchaseAvailabilityRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available_territories** | [**EndUserLicenseAgreementRelationshipsTerritories**](EndUserLicenseAgreementRelationshipsTerritories.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_availability_relationships import InAppPurchaseAvailabilityRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseAvailabilityRelationships from a JSON string
in_app_purchase_availability_relationships_instance = InAppPurchaseAvailabilityRelationships.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseAvailabilityRelationships.to_json())

# convert the object into a dict
in_app_purchase_availability_relationships_dict = in_app_purchase_availability_relationships_instance.to_dict()
# create an instance of InAppPurchaseAvailabilityRelationships from a dict
in_app_purchase_availability_relationships_from_dict = InAppPurchaseAvailabilityRelationships.from_dict(in_app_purchase_availability_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



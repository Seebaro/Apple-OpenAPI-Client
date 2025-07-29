# InAppPurchaseV2RelationshipsIapPriceSchedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**InAppPurchaseV2RelationshipsIapPriceScheduleData**](InAppPurchaseV2RelationshipsIapPriceScheduleData.md) |  | [optional] 

## Example

```python
from openapi_client.models.in_app_purchase_v2_relationships_iap_price_schedule import InAppPurchaseV2RelationshipsIapPriceSchedule

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2RelationshipsIapPriceSchedule from a JSON string
in_app_purchase_v2_relationships_iap_price_schedule_instance = InAppPurchaseV2RelationshipsIapPriceSchedule.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2RelationshipsIapPriceSchedule.to_json())

# convert the object into a dict
in_app_purchase_v2_relationships_iap_price_schedule_dict = in_app_purchase_v2_relationships_iap_price_schedule_instance.to_dict()
# create an instance of InAppPurchaseV2RelationshipsIapPriceSchedule from a dict
in_app_purchase_v2_relationships_iap_price_schedule_from_dict = InAppPurchaseV2RelationshipsIapPriceSchedule.from_dict(in_app_purchase_v2_relationships_iap_price_schedule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



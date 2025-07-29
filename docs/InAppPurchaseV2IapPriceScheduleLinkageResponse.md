# InAppPurchaseV2IapPriceScheduleLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InAppPurchaseV2RelationshipsIapPriceScheduleData**](InAppPurchaseV2RelationshipsIapPriceScheduleData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.in_app_purchase_v2_iap_price_schedule_linkage_response import InAppPurchaseV2IapPriceScheduleLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InAppPurchaseV2IapPriceScheduleLinkageResponse from a JSON string
in_app_purchase_v2_iap_price_schedule_linkage_response_instance = InAppPurchaseV2IapPriceScheduleLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(InAppPurchaseV2IapPriceScheduleLinkageResponse.to_json())

# convert the object into a dict
in_app_purchase_v2_iap_price_schedule_linkage_response_dict = in_app_purchase_v2_iap_price_schedule_linkage_response_instance.to_dict()
# create an instance of InAppPurchaseV2IapPriceScheduleLinkageResponse from a dict
in_app_purchase_v2_iap_price_schedule_linkage_response_from_dict = InAppPurchaseV2IapPriceScheduleLinkageResponse.from_dict(in_app_purchase_v2_iap_price_schedule_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



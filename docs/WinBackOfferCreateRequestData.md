# WinBackOfferCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**WinBackOfferCreateRequestDataAttributes**](WinBackOfferCreateRequestDataAttributes.md) |  | 
**relationships** | [**WinBackOfferCreateRequestDataRelationships**](WinBackOfferCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.win_back_offer_create_request_data import WinBackOfferCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferCreateRequestData from a JSON string
win_back_offer_create_request_data_instance = WinBackOfferCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferCreateRequestData.to_json())

# convert the object into a dict
win_back_offer_create_request_data_dict = win_back_offer_create_request_data_instance.to_dict()
# create an instance of WinBackOfferCreateRequestData from a dict
win_back_offer_create_request_data_from_dict = WinBackOfferCreateRequestData.from_dict(win_back_offer_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



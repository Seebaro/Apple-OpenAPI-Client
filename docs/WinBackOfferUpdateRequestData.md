# WinBackOfferUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**WinBackOfferUpdateRequestDataAttributes**](WinBackOfferUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.win_back_offer_update_request_data import WinBackOfferUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of WinBackOfferUpdateRequestData from a JSON string
win_back_offer_update_request_data_instance = WinBackOfferUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(WinBackOfferUpdateRequestData.to_json())

# convert the object into a dict
win_back_offer_update_request_data_dict = win_back_offer_update_request_data_instance.to_dict()
# create an instance of WinBackOfferUpdateRequestData from a dict
win_back_offer_update_request_data_from_dict = WinBackOfferUpdateRequestData.from_dict(win_back_offer_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



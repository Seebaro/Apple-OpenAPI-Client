# AppGameCenterDetailLinkageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AppRelationshipsGameCenterDetailData**](AppRelationshipsGameCenterDetailData.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.app_game_center_detail_linkage_response import AppGameCenterDetailLinkageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppGameCenterDetailLinkageResponse from a JSON string
app_game_center_detail_linkage_response_instance = AppGameCenterDetailLinkageResponse.from_json(json)
# print the JSON string representation of the object
print(AppGameCenterDetailLinkageResponse.to_json())

# convert the object into a dict
app_game_center_detail_linkage_response_dict = app_game_center_detail_linkage_response_instance.to_dict()
# create an instance of AppGameCenterDetailLinkageResponse from a dict
app_game_center_detail_linkage_response_from_dict = AppGameCenterDetailLinkageResponse.from_dict(app_game_center_detail_linkage_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



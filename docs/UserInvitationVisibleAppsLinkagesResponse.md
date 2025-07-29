# UserInvitationVisibleAppsLinkagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[AccessibilityDeclarationCreateRequestDataRelationshipsAppData]**](AccessibilityDeclarationCreateRequestDataRelationshipsAppData.md) |  | 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.user_invitation_visible_apps_linkages_response import UserInvitationVisibleAppsLinkagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserInvitationVisibleAppsLinkagesResponse from a JSON string
user_invitation_visible_apps_linkages_response_instance = UserInvitationVisibleAppsLinkagesResponse.from_json(json)
# print the JSON string representation of the object
print(UserInvitationVisibleAppsLinkagesResponse.to_json())

# convert the object into a dict
user_invitation_visible_apps_linkages_response_dict = user_invitation_visible_apps_linkages_response_instance.to_dict()
# create an instance of UserInvitationVisibleAppsLinkagesResponse from a dict
user_invitation_visible_apps_linkages_response_from_dict = UserInvitationVisibleAppsLinkagesResponse.from_dict(user_invitation_visible_apps_linkages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



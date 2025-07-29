# openapi_client.SubscriptionsApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subscriptions_app_store_review_screenshot_get_to_one_related**](SubscriptionsApi.md#subscriptions_app_store_review_screenshot_get_to_one_related) | **GET** /v1/subscriptions/{id}/appStoreReviewScreenshot | 
[**subscriptions_app_store_review_screenshot_get_to_one_relationship**](SubscriptionsApi.md#subscriptions_app_store_review_screenshot_get_to_one_relationship) | **GET** /v1/subscriptions/{id}/relationships/appStoreReviewScreenshot | 
[**subscriptions_create_instance**](SubscriptionsApi.md#subscriptions_create_instance) | **POST** /v1/subscriptions | 
[**subscriptions_delete_instance**](SubscriptionsApi.md#subscriptions_delete_instance) | **DELETE** /v1/subscriptions/{id} | 
[**subscriptions_get_instance**](SubscriptionsApi.md#subscriptions_get_instance) | **GET** /v1/subscriptions/{id} | 
[**subscriptions_images_get_to_many_related**](SubscriptionsApi.md#subscriptions_images_get_to_many_related) | **GET** /v1/subscriptions/{id}/images | 
[**subscriptions_images_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_images_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/images | 
[**subscriptions_introductory_offers_delete_to_many_relationship**](SubscriptionsApi.md#subscriptions_introductory_offers_delete_to_many_relationship) | **DELETE** /v1/subscriptions/{id}/relationships/introductoryOffers | 
[**subscriptions_introductory_offers_get_to_many_related**](SubscriptionsApi.md#subscriptions_introductory_offers_get_to_many_related) | **GET** /v1/subscriptions/{id}/introductoryOffers | 
[**subscriptions_introductory_offers_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_introductory_offers_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/introductoryOffers | 
[**subscriptions_offer_codes_get_to_many_related**](SubscriptionsApi.md#subscriptions_offer_codes_get_to_many_related) | **GET** /v1/subscriptions/{id}/offerCodes | 
[**subscriptions_offer_codes_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_offer_codes_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/offerCodes | 
[**subscriptions_price_points_get_to_many_related**](SubscriptionsApi.md#subscriptions_price_points_get_to_many_related) | **GET** /v1/subscriptions/{id}/pricePoints | 
[**subscriptions_price_points_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_price_points_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/pricePoints | 
[**subscriptions_prices_delete_to_many_relationship**](SubscriptionsApi.md#subscriptions_prices_delete_to_many_relationship) | **DELETE** /v1/subscriptions/{id}/relationships/prices | 
[**subscriptions_prices_get_to_many_related**](SubscriptionsApi.md#subscriptions_prices_get_to_many_related) | **GET** /v1/subscriptions/{id}/prices | 
[**subscriptions_prices_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_prices_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/prices | 
[**subscriptions_promoted_purchase_get_to_one_related**](SubscriptionsApi.md#subscriptions_promoted_purchase_get_to_one_related) | **GET** /v1/subscriptions/{id}/promotedPurchase | 
[**subscriptions_promoted_purchase_get_to_one_relationship**](SubscriptionsApi.md#subscriptions_promoted_purchase_get_to_one_relationship) | **GET** /v1/subscriptions/{id}/relationships/promotedPurchase | 
[**subscriptions_promotional_offers_get_to_many_related**](SubscriptionsApi.md#subscriptions_promotional_offers_get_to_many_related) | **GET** /v1/subscriptions/{id}/promotionalOffers | 
[**subscriptions_promotional_offers_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_promotional_offers_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/promotionalOffers | 
[**subscriptions_subscription_availability_get_to_one_related**](SubscriptionsApi.md#subscriptions_subscription_availability_get_to_one_related) | **GET** /v1/subscriptions/{id}/subscriptionAvailability | 
[**subscriptions_subscription_availability_get_to_one_relationship**](SubscriptionsApi.md#subscriptions_subscription_availability_get_to_one_relationship) | **GET** /v1/subscriptions/{id}/relationships/subscriptionAvailability | 
[**subscriptions_subscription_localizations_get_to_many_related**](SubscriptionsApi.md#subscriptions_subscription_localizations_get_to_many_related) | **GET** /v1/subscriptions/{id}/subscriptionLocalizations | 
[**subscriptions_subscription_localizations_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_subscription_localizations_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/subscriptionLocalizations | 
[**subscriptions_update_instance**](SubscriptionsApi.md#subscriptions_update_instance) | **PATCH** /v1/subscriptions/{id} | 
[**subscriptions_win_back_offers_get_to_many_related**](SubscriptionsApi.md#subscriptions_win_back_offers_get_to_many_related) | **GET** /v1/subscriptions/{id}/winBackOffers | 
[**subscriptions_win_back_offers_get_to_many_relationship**](SubscriptionsApi.md#subscriptions_win_back_offers_get_to_many_relationship) | **GET** /v1/subscriptions/{id}/relationships/winBackOffers | 


# **subscriptions_app_store_review_screenshot_get_to_one_related**
> SubscriptionAppStoreReviewScreenshotResponse subscriptions_app_store_review_screenshot_get_to_one_related(id, fields_subscription_app_store_review_screenshots=fields_subscription_app_store_review_screenshots, fields_subscriptions=fields_subscriptions, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_app_store_review_screenshot_response import SubscriptionAppStoreReviewScreenshotResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_app_store_review_screenshots = ['fields_subscription_app_store_review_screenshots_example'] # List[str] | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscriptions_app_store_review_screenshot_get_to_one_related(id, fields_subscription_app_store_review_screenshots=fields_subscription_app_store_review_screenshots, fields_subscriptions=fields_subscriptions, include=include)
        print("The response of SubscriptionsApi->subscriptions_app_store_review_screenshot_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_app_store_review_screenshot_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_app_store_review_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionAppStoreReviewScreenshotResponse**](SubscriptionAppStoreReviewScreenshotResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single SubscriptionAppStoreReviewScreenshot |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_app_store_review_screenshot_get_to_one_relationship**
> SubscriptionAppStoreReviewScreenshotLinkageResponse subscriptions_app_store_review_screenshot_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_app_store_review_screenshot_linkage_response import SubscriptionAppStoreReviewScreenshotLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.subscriptions_app_store_review_screenshot_get_to_one_relationship(id)
        print("The response of SubscriptionsApi->subscriptions_app_store_review_screenshot_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_app_store_review_screenshot_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**SubscriptionAppStoreReviewScreenshotLinkageResponse**](SubscriptionAppStoreReviewScreenshotLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_create_instance**
> SubscriptionResponse subscriptions_create_instance(subscription_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_create_request import SubscriptionCreateRequest
from openapi_client.models.subscription_response import SubscriptionResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    subscription_create_request = openapi_client.SubscriptionCreateRequest() # SubscriptionCreateRequest | Subscription representation

    try:
        api_response = api_instance.subscriptions_create_instance(subscription_create_request)
        print("The response of SubscriptionsApi->subscriptions_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscription_create_request** | [**SubscriptionCreateRequest**](SubscriptionCreateRequest.md)| Subscription representation | 

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**201** | Single Subscription |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_delete_instance**
> subscriptions_delete_instance(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.subscriptions_delete_instance(id)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_delete_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_get_instance**
> SubscriptionResponse subscriptions_get_instance(id, fields_subscriptions=fields_subscriptions, fields_subscription_localizations=fields_subscription_localizations, fields_subscription_app_store_review_screenshots=fields_subscription_app_store_review_screenshots, fields_subscription_introductory_offers=fields_subscription_introductory_offers, fields_subscription_promotional_offers=fields_subscription_promotional_offers, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscription_prices=fields_subscription_prices, fields_promoted_purchases=fields_promoted_purchases, fields_subscription_availabilities=fields_subscription_availabilities, fields_win_back_offers=fields_win_back_offers, fields_subscription_images=fields_subscription_images, include=include, limit_images=limit_images, limit_introductory_offers=limit_introductory_offers, limit_offer_codes=limit_offer_codes, limit_prices=limit_prices, limit_promotional_offers=limit_promotional_offers, limit_subscription_localizations=limit_subscription_localizations, limit_win_back_offers=limit_win_back_offers)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_response import SubscriptionResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    fields_subscription_localizations = ['fields_subscription_localizations_example'] # List[str] | the fields to include for returned resources of type subscriptionLocalizations (optional)
    fields_subscription_app_store_review_screenshots = ['fields_subscription_app_store_review_screenshots_example'] # List[str] | the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots (optional)
    fields_subscription_introductory_offers = ['fields_subscription_introductory_offers_example'] # List[str] | the fields to include for returned resources of type subscriptionIntroductoryOffers (optional)
    fields_subscription_promotional_offers = ['fields_subscription_promotional_offers_example'] # List[str] | the fields to include for returned resources of type subscriptionPromotionalOffers (optional)
    fields_subscription_offer_codes = ['fields_subscription_offer_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodes (optional)
    fields_subscription_prices = ['fields_subscription_prices_example'] # List[str] | the fields to include for returned resources of type subscriptionPrices (optional)
    fields_promoted_purchases = ['fields_promoted_purchases_example'] # List[str] | the fields to include for returned resources of type promotedPurchases (optional)
    fields_subscription_availabilities = ['fields_subscription_availabilities_example'] # List[str] | the fields to include for returned resources of type subscriptionAvailabilities (optional)
    fields_win_back_offers = ['fields_win_back_offers_example'] # List[str] | the fields to include for returned resources of type winBackOffers (optional)
    fields_subscription_images = ['fields_subscription_images_example'] # List[str] | the fields to include for returned resources of type subscriptionImages (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_images = 56 # int | maximum number of related images returned (when they are included) (optional)
    limit_introductory_offers = 56 # int | maximum number of related introductoryOffers returned (when they are included) (optional)
    limit_offer_codes = 56 # int | maximum number of related offerCodes returned (when they are included) (optional)
    limit_prices = 56 # int | maximum number of related prices returned (when they are included) (optional)
    limit_promotional_offers = 56 # int | maximum number of related promotionalOffers returned (when they are included) (optional)
    limit_subscription_localizations = 56 # int | maximum number of related subscriptionLocalizations returned (when they are included) (optional)
    limit_win_back_offers = 56 # int | maximum number of related winBackOffers returned (when they are included) (optional)

    try:
        api_response = api_instance.subscriptions_get_instance(id, fields_subscriptions=fields_subscriptions, fields_subscription_localizations=fields_subscription_localizations, fields_subscription_app_store_review_screenshots=fields_subscription_app_store_review_screenshots, fields_subscription_introductory_offers=fields_subscription_introductory_offers, fields_subscription_promotional_offers=fields_subscription_promotional_offers, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscription_prices=fields_subscription_prices, fields_promoted_purchases=fields_promoted_purchases, fields_subscription_availabilities=fields_subscription_availabilities, fields_win_back_offers=fields_win_back_offers, fields_subscription_images=fields_subscription_images, include=include, limit_images=limit_images, limit_introductory_offers=limit_introductory_offers, limit_offer_codes=limit_offer_codes, limit_prices=limit_prices, limit_promotional_offers=limit_promotional_offers, limit_subscription_localizations=limit_subscription_localizations, limit_win_back_offers=limit_win_back_offers)
        print("The response of SubscriptionsApi->subscriptions_get_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_get_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **fields_subscription_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionLocalizations | [optional] 
 **fields_subscription_app_store_review_screenshots** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionAppStoreReviewScreenshots | [optional] 
 **fields_subscription_introductory_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional] 
 **fields_subscription_promotional_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPromotionalOffers | [optional] 
 **fields_subscription_offer_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodes | [optional] 
 **fields_subscription_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPrices | [optional] 
 **fields_promoted_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type promotedPurchases | [optional] 
 **fields_subscription_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionAvailabilities | [optional] 
 **fields_win_back_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type winBackOffers | [optional] 
 **fields_subscription_images** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionImages | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_images** | **int**| maximum number of related images returned (when they are included) | [optional] 
 **limit_introductory_offers** | **int**| maximum number of related introductoryOffers returned (when they are included) | [optional] 
 **limit_offer_codes** | **int**| maximum number of related offerCodes returned (when they are included) | [optional] 
 **limit_prices** | **int**| maximum number of related prices returned (when they are included) | [optional] 
 **limit_promotional_offers** | **int**| maximum number of related promotionalOffers returned (when they are included) | [optional] 
 **limit_subscription_localizations** | **int**| maximum number of related subscriptionLocalizations returned (when they are included) | [optional] 
 **limit_win_back_offers** | **int**| maximum number of related winBackOffers returned (when they are included) | [optional] 

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single Subscription |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_images_get_to_many_related**
> SubscriptionImagesResponse subscriptions_images_get_to_many_related(id, fields_subscription_images=fields_subscription_images, fields_subscriptions=fields_subscriptions, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_images_response import SubscriptionImagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_images = ['fields_subscription_images_example'] # List[str] | the fields to include for returned resources of type subscriptionImages (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscriptions_images_get_to_many_related(id, fields_subscription_images=fields_subscription_images, fields_subscriptions=fields_subscriptions, limit=limit, include=include)
        print("The response of SubscriptionsApi->subscriptions_images_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_images_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_images** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionImages | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionImagesResponse**](SubscriptionImagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionImages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_images_get_to_many_relationship**
> SubscriptionImagesLinkagesResponse subscriptions_images_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_images_linkages_response import SubscriptionImagesLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_images_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_images_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_images_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionImagesLinkagesResponse**](SubscriptionImagesLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_introductory_offers_delete_to_many_relationship**
> subscriptions_introductory_offers_delete_to_many_relationship(id, subscription_introductory_offers_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_introductory_offers_linkages_request import SubscriptionIntroductoryOffersLinkagesRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_introductory_offers_linkages_request = openapi_client.SubscriptionIntroductoryOffersLinkagesRequest() # SubscriptionIntroductoryOffersLinkagesRequest | List of related linkages

    try:
        api_instance.subscriptions_introductory_offers_delete_to_many_relationship(id, subscription_introductory_offers_linkages_request)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_introductory_offers_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_introductory_offers_linkages_request** | [**SubscriptionIntroductoryOffersLinkagesRequest**](SubscriptionIntroductoryOffersLinkagesRequest.md)| List of related linkages | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_introductory_offers_get_to_many_related**
> SubscriptionIntroductoryOffersResponse subscriptions_introductory_offers_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_introductory_offers=fields_subscription_introductory_offers, fields_subscriptions=fields_subscriptions, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_introductory_offers_response import SubscriptionIntroductoryOffersResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_subscription_introductory_offers = ['fields_subscription_introductory_offers_example'] # List[str] | the fields to include for returned resources of type subscriptionIntroductoryOffers (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    fields_subscription_price_points = ['fields_subscription_price_points_example'] # List[str] | the fields to include for returned resources of type subscriptionPricePoints (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscriptions_introductory_offers_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_introductory_offers=fields_subscription_introductory_offers, fields_subscriptions=fields_subscriptions, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)
        print("The response of SubscriptionsApi->subscriptions_introductory_offers_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_introductory_offers_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_subscription_introductory_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionIntroductoryOffers | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **fields_subscription_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPricePoints | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionIntroductoryOffersResponse**](SubscriptionIntroductoryOffersResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionIntroductoryOffers |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_introductory_offers_get_to_many_relationship**
> SubscriptionIntroductoryOffersLinkagesResponse subscriptions_introductory_offers_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_introductory_offers_linkages_response import SubscriptionIntroductoryOffersLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_introductory_offers_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_introductory_offers_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_introductory_offers_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionIntroductoryOffersLinkagesResponse**](SubscriptionIntroductoryOffersLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_offer_codes_get_to_many_related**
> SubscriptionOfferCodesResponse subscriptions_offer_codes_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscriptions=fields_subscriptions, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, fields_subscription_offer_code_prices=fields_subscription_offer_code_prices, limit=limit, include=include, limit_one_time_use_codes=limit_one_time_use_codes, limit_custom_codes=limit_custom_codes, limit_prices=limit_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_codes_response import SubscriptionOfferCodesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by territory (optional)
    fields_subscription_offer_codes = ['fields_subscription_offer_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodes (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    fields_subscription_offer_code_one_time_use_codes = ['fields_subscription_offer_code_one_time_use_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes (optional)
    fields_subscription_offer_code_custom_codes = ['fields_subscription_offer_code_custom_codes_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodeCustomCodes (optional)
    fields_subscription_offer_code_prices = ['fields_subscription_offer_code_prices_example'] # List[str] | the fields to include for returned resources of type subscriptionOfferCodePrices (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_one_time_use_codes = 56 # int | maximum number of related oneTimeUseCodes returned (when they are included) (optional)
    limit_custom_codes = 56 # int | maximum number of related customCodes returned (when they are included) (optional)
    limit_prices = 56 # int | maximum number of related prices returned (when they are included) (optional)

    try:
        api_response = api_instance.subscriptions_offer_codes_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_offer_codes=fields_subscription_offer_codes, fields_subscriptions=fields_subscriptions, fields_subscription_offer_code_one_time_use_codes=fields_subscription_offer_code_one_time_use_codes, fields_subscription_offer_code_custom_codes=fields_subscription_offer_code_custom_codes, fields_subscription_offer_code_prices=fields_subscription_offer_code_prices, limit=limit, include=include, limit_one_time_use_codes=limit_one_time_use_codes, limit_custom_codes=limit_custom_codes, limit_prices=limit_prices)
        print("The response of SubscriptionsApi->subscriptions_offer_codes_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_offer_codes_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by territory | [optional] 
 **fields_subscription_offer_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodes | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **fields_subscription_offer_code_one_time_use_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeOneTimeUseCodes | [optional] 
 **fields_subscription_offer_code_custom_codes** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodeCustomCodes | [optional] 
 **fields_subscription_offer_code_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionOfferCodePrices | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_one_time_use_codes** | **int**| maximum number of related oneTimeUseCodes returned (when they are included) | [optional] 
 **limit_custom_codes** | **int**| maximum number of related customCodes returned (when they are included) | [optional] 
 **limit_prices** | **int**| maximum number of related prices returned (when they are included) | [optional] 

### Return type

[**SubscriptionOfferCodesResponse**](SubscriptionOfferCodesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionOfferCodes |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_offer_codes_get_to_many_relationship**
> SubscriptionOfferCodesLinkagesResponse subscriptions_offer_codes_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_offer_codes_linkages_response import SubscriptionOfferCodesLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_offer_codes_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_offer_codes_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_offer_codes_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionOfferCodesLinkagesResponse**](SubscriptionOfferCodesLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_price_points_get_to_many_related**
> SubscriptionPricePointsResponse subscriptions_price_points_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_price_points=fields_subscription_price_points, fields_territories=fields_territories, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_price_points_response import SubscriptionPricePointsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_subscription_price_points = ['fields_subscription_price_points_example'] # List[str] | the fields to include for returned resources of type subscriptionPricePoints (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscriptions_price_points_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_price_points=fields_subscription_price_points, fields_territories=fields_territories, limit=limit, include=include)
        print("The response of SubscriptionsApi->subscriptions_price_points_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_price_points_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_subscription_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPricePoints | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionPricePointsResponse**](SubscriptionPricePointsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/csv

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionPricePoints |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_price_points_get_to_many_relationship**
> SubscriptionPricePointsLinkagesResponse subscriptions_price_points_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_price_points_linkages_response import SubscriptionPricePointsLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_price_points_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_price_points_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_price_points_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionPricePointsLinkagesResponse**](SubscriptionPricePointsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_prices_delete_to_many_relationship**
> subscriptions_prices_delete_to_many_relationship(id, subscription_prices_linkages_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_prices_linkages_request import SubscriptionPricesLinkagesRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_prices_linkages_request = openapi_client.SubscriptionPricesLinkagesRequest() # SubscriptionPricesLinkagesRequest | List of related linkages

    try:
        api_instance.subscriptions_prices_delete_to_many_relationship(id, subscription_prices_linkages_request)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_prices_delete_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_prices_linkages_request** | [**SubscriptionPricesLinkagesRequest**](SubscriptionPricesLinkagesRequest.md)| List of related linkages | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_prices_get_to_many_related**
> SubscriptionPricesResponse subscriptions_prices_get_to_many_related(id, filter_subscription_price_point=filter_subscription_price_point, filter_territory=filter_territory, fields_subscription_prices=fields_subscription_prices, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_prices_response import SubscriptionPricesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_subscription_price_point = ['filter_subscription_price_point_example'] # List[str] | filter by id(s) of related 'subscriptionPricePoint' (optional)
    filter_territory = ['filter_territory_example'] # List[str] | filter by id(s) of related 'territory' (optional)
    fields_subscription_prices = ['fields_subscription_prices_example'] # List[str] | the fields to include for returned resources of type subscriptionPrices (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    fields_subscription_price_points = ['fields_subscription_price_points_example'] # List[str] | the fields to include for returned resources of type subscriptionPricePoints (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscriptions_prices_get_to_many_related(id, filter_subscription_price_point=filter_subscription_price_point, filter_territory=filter_territory, fields_subscription_prices=fields_subscription_prices, fields_territories=fields_territories, fields_subscription_price_points=fields_subscription_price_points, limit=limit, include=include)
        print("The response of SubscriptionsApi->subscriptions_prices_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_prices_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_subscription_price_point** | [**List[str]**](str.md)| filter by id(s) of related &#39;subscriptionPricePoint&#39; | [optional] 
 **filter_territory** | [**List[str]**](str.md)| filter by id(s) of related &#39;territory&#39; | [optional] 
 **fields_subscription_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPrices | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **fields_subscription_price_points** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPricePoints | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionPricesResponse**](SubscriptionPricesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionPrices |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_prices_get_to_many_relationship**
> SubscriptionPricesLinkagesResponse subscriptions_prices_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_prices_linkages_response import SubscriptionPricesLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_prices_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_prices_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_prices_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionPricesLinkagesResponse**](SubscriptionPricesLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_promoted_purchase_get_to_one_related**
> PromotedPurchaseResponse subscriptions_promoted_purchase_get_to_one_related(id, fields_promoted_purchases=fields_promoted_purchases, fields_in_app_purchases=fields_in_app_purchases, fields_subscriptions=fields_subscriptions, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.promoted_purchase_response import PromotedPurchaseResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_promoted_purchases = ['fields_promoted_purchases_example'] # List[str] | the fields to include for returned resources of type promotedPurchases (optional)
    fields_in_app_purchases = ['fields_in_app_purchases_example'] # List[str] | the fields to include for returned resources of type inAppPurchases (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscriptions_promoted_purchase_get_to_one_related(id, fields_promoted_purchases=fields_promoted_purchases, fields_in_app_purchases=fields_in_app_purchases, fields_subscriptions=fields_subscriptions, include=include)
        print("The response of SubscriptionsApi->subscriptions_promoted_purchase_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_promoted_purchase_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_promoted_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type promotedPurchases | [optional] 
 **fields_in_app_purchases** | [**List[str]**](str.md)| the fields to include for returned resources of type inAppPurchases | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**PromotedPurchaseResponse**](PromotedPurchaseResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single PromotedPurchase |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_promoted_purchase_get_to_one_relationship**
> SubscriptionPromotedPurchaseLinkageResponse subscriptions_promoted_purchase_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_promoted_purchase_linkage_response import SubscriptionPromotedPurchaseLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.subscriptions_promoted_purchase_get_to_one_relationship(id)
        print("The response of SubscriptionsApi->subscriptions_promoted_purchase_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_promoted_purchase_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**SubscriptionPromotedPurchaseLinkageResponse**](SubscriptionPromotedPurchaseLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_promotional_offers_get_to_many_related**
> SubscriptionPromotionalOffersResponse subscriptions_promotional_offers_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_promotional_offers=fields_subscription_promotional_offers, fields_subscriptions=fields_subscriptions, fields_subscription_promotional_offer_prices=fields_subscription_promotional_offer_prices, limit=limit, include=include, limit_prices=limit_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_promotional_offers_response import SubscriptionPromotionalOffersResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    filter_territory = ['filter_territory_example'] # List[str] | filter by territory (optional)
    fields_subscription_promotional_offers = ['fields_subscription_promotional_offers_example'] # List[str] | the fields to include for returned resources of type subscriptionPromotionalOffers (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    fields_subscription_promotional_offer_prices = ['fields_subscription_promotional_offer_prices_example'] # List[str] | the fields to include for returned resources of type subscriptionPromotionalOfferPrices (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_prices = 56 # int | maximum number of related prices returned (when they are included) (optional)

    try:
        api_response = api_instance.subscriptions_promotional_offers_get_to_many_related(id, filter_territory=filter_territory, fields_subscription_promotional_offers=fields_subscription_promotional_offers, fields_subscriptions=fields_subscriptions, fields_subscription_promotional_offer_prices=fields_subscription_promotional_offer_prices, limit=limit, include=include, limit_prices=limit_prices)
        print("The response of SubscriptionsApi->subscriptions_promotional_offers_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_promotional_offers_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **filter_territory** | [**List[str]**](str.md)| filter by territory | [optional] 
 **fields_subscription_promotional_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPromotionalOffers | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **fields_subscription_promotional_offer_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionPromotionalOfferPrices | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_prices** | **int**| maximum number of related prices returned (when they are included) | [optional] 

### Return type

[**SubscriptionPromotionalOffersResponse**](SubscriptionPromotionalOffersResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionPromotionalOffers |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_promotional_offers_get_to_many_relationship**
> SubscriptionPromotionalOffersLinkagesResponse subscriptions_promotional_offers_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_promotional_offers_linkages_response import SubscriptionPromotionalOffersLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_promotional_offers_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_promotional_offers_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_promotional_offers_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionPromotionalOffersLinkagesResponse**](SubscriptionPromotionalOffersLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_subscription_availability_get_to_one_related**
> SubscriptionAvailabilityResponse subscriptions_subscription_availability_get_to_one_related(id, fields_subscription_availabilities=fields_subscription_availabilities, fields_territories=fields_territories, include=include, limit_available_territories=limit_available_territories)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_availability_response import SubscriptionAvailabilityResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_availabilities = ['fields_subscription_availabilities_example'] # List[str] | the fields to include for returned resources of type subscriptionAvailabilities (optional)
    fields_territories = ['fields_territories_example'] # List[str] | the fields to include for returned resources of type territories (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_available_territories = 56 # int | maximum number of related availableTerritories returned (when they are included) (optional)

    try:
        api_response = api_instance.subscriptions_subscription_availability_get_to_one_related(id, fields_subscription_availabilities=fields_subscription_availabilities, fields_territories=fields_territories, include=include, limit_available_territories=limit_available_territories)
        print("The response of SubscriptionsApi->subscriptions_subscription_availability_get_to_one_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_subscription_availability_get_to_one_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_availabilities** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionAvailabilities | [optional] 
 **fields_territories** | [**List[str]**](str.md)| the fields to include for returned resources of type territories | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_available_territories** | **int**| maximum number of related availableTerritories returned (when they are included) | [optional] 

### Return type

[**SubscriptionAvailabilityResponse**](SubscriptionAvailabilityResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Single SubscriptionAvailability |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_subscription_availability_get_to_one_relationship**
> SubscriptionSubscriptionAvailabilityLinkageResponse subscriptions_subscription_availability_get_to_one_relationship(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_subscription_availability_linkage_response import SubscriptionSubscriptionAvailabilityLinkageResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_response = api_instance.subscriptions_subscription_availability_get_to_one_relationship(id)
        print("The response of SubscriptionsApi->subscriptions_subscription_availability_get_to_one_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_subscription_availability_get_to_one_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

[**SubscriptionSubscriptionAvailabilityLinkageResponse**](SubscriptionSubscriptionAvailabilityLinkageResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | Related linkage |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_subscription_localizations_get_to_many_related**
> SubscriptionLocalizationsResponse subscriptions_subscription_localizations_get_to_many_related(id, fields_subscription_localizations=fields_subscription_localizations, fields_subscriptions=fields_subscriptions, limit=limit, include=include)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_localizations_response import SubscriptionLocalizationsResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_subscription_localizations = ['fields_subscription_localizations_example'] # List[str] | the fields to include for returned resources of type subscriptionLocalizations (optional)
    fields_subscriptions = ['fields_subscriptions_example'] # List[str] | the fields to include for returned resources of type subscriptions (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)

    try:
        api_response = api_instance.subscriptions_subscription_localizations_get_to_many_related(id, fields_subscription_localizations=fields_subscription_localizations, fields_subscriptions=fields_subscriptions, limit=limit, include=include)
        print("The response of SubscriptionsApi->subscriptions_subscription_localizations_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_subscription_localizations_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_subscription_localizations** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptionLocalizations | [optional] 
 **fields_subscriptions** | [**List[str]**](str.md)| the fields to include for returned resources of type subscriptions | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 

### Return type

[**SubscriptionLocalizationsResponse**](SubscriptionLocalizationsResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of SubscriptionLocalizations |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_subscription_localizations_get_to_many_relationship**
> SubscriptionSubscriptionLocalizationsLinkagesResponse subscriptions_subscription_localizations_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_subscription_localizations_linkages_response import SubscriptionSubscriptionLocalizationsLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_subscription_localizations_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_subscription_localizations_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_subscription_localizations_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionSubscriptionLocalizationsLinkagesResponse**](SubscriptionSubscriptionLocalizationsLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_update_instance**
> SubscriptionResponse subscriptions_update_instance(id, subscription_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_response import SubscriptionResponse
from openapi_client.models.subscription_update_request import SubscriptionUpdateRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    subscription_update_request = openapi_client.SubscriptionUpdateRequest() # SubscriptionUpdateRequest | Subscription representation

    try:
        api_response = api_instance.subscriptions_update_instance(id, subscription_update_request)
        print("The response of SubscriptionsApi->subscriptions_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **subscription_update_request** | [**SubscriptionUpdateRequest**](SubscriptionUpdateRequest.md)| Subscription representation | 

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**200** | Single Subscription |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_win_back_offers_get_to_many_related**
> WinBackOffersResponse subscriptions_win_back_offers_get_to_many_related(id, fields_win_back_offers=fields_win_back_offers, fields_win_back_offer_prices=fields_win_back_offer_prices, limit=limit, include=include, limit_prices=limit_prices)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.win_back_offers_response import WinBackOffersResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    fields_win_back_offers = ['fields_win_back_offers_example'] # List[str] | the fields to include for returned resources of type winBackOffers (optional)
    fields_win_back_offer_prices = ['fields_win_back_offer_prices_example'] # List[str] | the fields to include for returned resources of type winBackOfferPrices (optional)
    limit = 56 # int | maximum resources per page (optional)
    include = ['include_example'] # List[str] | comma-separated list of relationships to include (optional)
    limit_prices = 56 # int | maximum number of related prices returned (when they are included) (optional)

    try:
        api_response = api_instance.subscriptions_win_back_offers_get_to_many_related(id, fields_win_back_offers=fields_win_back_offers, fields_win_back_offer_prices=fields_win_back_offer_prices, limit=limit, include=include, limit_prices=limit_prices)
        print("The response of SubscriptionsApi->subscriptions_win_back_offers_get_to_many_related:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_win_back_offers_get_to_many_related: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **fields_win_back_offers** | [**List[str]**](str.md)| the fields to include for returned resources of type winBackOffers | [optional] 
 **fields_win_back_offer_prices** | [**List[str]**](str.md)| the fields to include for returned resources of type winBackOfferPrices | [optional] 
 **limit** | **int**| maximum resources per page | [optional] 
 **include** | [**List[str]**](str.md)| comma-separated list of relationships to include | [optional] 
 **limit_prices** | **int**| maximum number of related prices returned (when they are included) | [optional] 

### Return type

[**WinBackOffersResponse**](WinBackOffersResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of WinBackOffers |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subscriptions_win_back_offers_get_to_many_relationship**
> SubscriptionWinBackOffersLinkagesResponse subscriptions_win_back_offers_get_to_many_relationship(id, limit=limit)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.subscription_win_back_offers_linkages_response import SubscriptionWinBackOffersLinkagesResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.SubscriptionsApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    limit = 56 # int | maximum resources per page (optional)

    try:
        api_response = api_instance.subscriptions_win_back_offers_get_to_many_relationship(id, limit=limit)
        print("The response of SubscriptionsApi->subscriptions_win_back_offers_get_to_many_relationship:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubscriptionsApi->subscriptions_win_back_offers_get_to_many_relationship: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **limit** | **int**| maximum resources per page | [optional] 

### Return type

[**SubscriptionWinBackOffersLinkagesResponse**](SubscriptionWinBackOffersLinkagesResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**200** | List of related linkages |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


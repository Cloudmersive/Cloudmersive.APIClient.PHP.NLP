# Swagger\Client\ExtractEntitiesApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**extractEntitiesPost**](ExtractEntitiesApi.md#extractEntitiesPost) | **POST** /nlp-v2/extract-entities | Extract entities from string


# **extractEntitiesPost**
> \Swagger\Client\Model\ExtractEntitiesResponse extractEntitiesPost($value)

Extract entities from string

Extract the named entitites from an input string.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\ExtractEntitiesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$value = new \Swagger\Client\Model\ExtractEntitiesRequest(); // \Swagger\Client\Model\ExtractEntitiesRequest | Input string

try {
    $result = $apiInstance->extractEntitiesPost($value);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ExtractEntitiesApi->extractEntitiesPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | [**\Swagger\Client\Model\ExtractEntitiesRequest**](../Model/ExtractEntitiesRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\ExtractEntitiesResponse**](../Model/ExtractEntitiesResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


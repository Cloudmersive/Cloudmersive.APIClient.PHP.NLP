# Swagger\Client\SegmentationApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**segmentationGetSentences**](SegmentationApi.md#segmentationGetSentences) | **POST** /nlp-v2/segmentation/sentences | Extract sentences from string
[**segmentationGetWords**](SegmentationApi.md#segmentationGetWords) | **POST** /nlp-v2/segmentation/words | Get words in input string


# **segmentationGetSentences**
> \Swagger\Client\Model\SentenceSegmentationResponse segmentationGetSentences($input)

Extract sentences from string

Segment an input string into separate sentences, output result as a string.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\SegmentationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\SentenceSegmentationRequest(); // \Swagger\Client\Model\SentenceSegmentationRequest | Input string

try {
    $result = $apiInstance->segmentationGetSentences($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SegmentationApi->segmentationGetSentences: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\SentenceSegmentationRequest**](../Model/SentenceSegmentationRequest.md)| Input string |

### Return type

[**\Swagger\Client\Model\SentenceSegmentationResponse**](../Model/SentenceSegmentationResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **segmentationGetWords**
> \Swagger\Client\Model\GetWordsResponse segmentationGetWords($input)

Get words in input string

Get the component words in an input string

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\SegmentationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\GetWordsRequest(); // \Swagger\Client\Model\GetWordsRequest | String to process

try {
    $result = $apiInstance->segmentationGetWords($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SegmentationApi->segmentationGetWords: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\GetWordsRequest**](../Model/GetWordsRequest.md)| String to process |

### Return type

[**\Swagger\Client\Model\GetWordsResponse**](../Model/GetWordsResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


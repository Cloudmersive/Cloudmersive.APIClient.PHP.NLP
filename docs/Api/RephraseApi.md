# Swagger\Client\RephraseApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**rephraseEnglishRephraseSentenceBySentence**](RephraseApi.md#rephraseEnglishRephraseSentenceBySentence) | **POST** /nlp-v2/rephrase/rephrase/eng/by-sentence | Rephrase, paraphrase English text sentence-by-sentence using Deep Learning AI


# **rephraseEnglishRephraseSentenceBySentence**
> \Swagger\Client\Model\RephraseResponse rephraseEnglishRephraseSentenceBySentence($input)

Rephrase, paraphrase English text sentence-by-sentence using Deep Learning AI

Automatically rephrases or paraphrases input text in English sentence by sentence using advanced Deep Learning and Neural NLP.  Creates multiple reprhasing candidates per input sentence, from 1 to 10 possible rephrasings of the original sentence.  Seeks to preserve original semantic meaning in rephrased output candidates.  Consumes 1-2 API calls per output rephrasing option generated, per sentence.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: Apikey
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Apikey', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Apikey', 'Bearer');

$apiInstance = new Swagger\Client\Api\RephraseApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$input = new \Swagger\Client\Model\RephraseRequest(); // \Swagger\Client\Model\RephraseRequest | Input rephrase request

try {
    $result = $apiInstance->rephraseEnglishRephraseSentenceBySentence($input);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RephraseApi->rephraseEnglishRephraseSentenceBySentence: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**\Swagger\Client\Model\RephraseRequest**](../Model/RephraseRequest.md)| Input rephrase request |

### Return type

[**\Swagger\Client\Model\RephraseResponse**](../Model/RephraseResponse.md)

### Authorization

[Apikey](../../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/xml, text/xml, application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


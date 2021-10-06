# How to use Collect API ?

* You need to extract Cryptken Encrypted Text from QR or Cryptken File.
* If payer is using Cryptken File, you just extract text from the file.
* If payer is using QR Code, you need to Scan QR Code and fetch the acquired URL, it returns JSON result with the format {"success":Boolean,"qr":String}, where qr represents Cryptken.
* Once you got Cryptken Encrypted Text, you need to make a post request to the end point, follow the instruction above.
* You must include two form data inside POST body, apiKey and cryptken.
* You can test with sandbox cryptken and replace with real cryptken when you start api as production.
* There is a failure limit on each end point, be careful not to be blocked your apiKey with high rate of failure requests.

## End Point
`https://api.cryptken.com/api-collect/cryptken`

## Method
`POST`

## Header
`content-type` : `application/x-www-form-urlencoded`


## Form Data
{`apiKey` : `your api key`, `cryptken` : `sandbox_test_cryptken` }

## Test API at
`https://www.cryptken.com/api` ! login required

## Result Display
![image](https://user-images.githubusercontent.com/92026194/136188605-b807645b-bc9f-4eb4-af0e-9abdd5de285e.png)

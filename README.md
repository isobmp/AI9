# AI9
Artificial Intelligence to change the way robots communicate with humans.

## API URL
http://api.brainshop.ai/get?bid=169494&key=zV3Ir2zUtvbEkGXa&uid=[uid]&msg=[msg]

Change the `[msg]` to any value, and the API will return a response.

### Parameters
* bid: The brain ID.
* key: The access key for the brain.
* uid: The ID you assign to end user， an alphanumeric text string.
* msg: The message from user.

Return Values
The API returns a JSON string structured as below
```
{
  "cnt":"[value]"
}
```
The JSON includes only one datum, 'cnt', the content of reply given by the brain. The reason to use JSON for a single datum here is we are extending the API and it will deliver more data in the future. The below is an example of possible JSON with more data.
```
{
  "cnt":"[value]",
  "scr":"[value]",
  "tts":"[value]",
  "face":"[value]"
}
```
To display the reply to end users, you need to convert JSON to an object or array (decoding) and then extract the content from the "cnt" data. You may search for the specific method to decode a JSON in your programming language.

# smartucapi
A simple and short API for UCS server made by Alpha Man

___

## Usage

1 First run this script locally on your machine
2 Go to your localhost with this url : 

`http://localhost/?give=key`

3 It will generate a code, copy that and paste it in your ucs.config file
4 Now turn your server on and again go to this url : 

`http://localhost/?get={thecodegenerated}&show=onlineplayer`

5 This above URI will show the amount of people playing in that server
6 To get the status of the server, change the `show` parameter to `status`

`http://localhost/?get={thecodegenerated}&show=status`

7 While the above code shows the status of the server.
___

### Available parameters

|Request|URI|Parameter|Description|
|-------|---|---------|-----------|
|`GET`|http://yourwebsite.com/apiv1|`/?give=key`|Outputs a string of 25 characters|
|`GET`|http://yourwebsite.com/apiv1|`/?get=key`|Script gets the key and searches for the input from UCS|
|`GET`|http://yourwebsite.com/apiv1|`/?get={yourkey}&show=onlineplayers`|Replace `{yourkey}` with your key and you will get the online players in your UCS|
|`GET`|http://yourwebsite.com/apiv1|`/?get={yourkey}&show=status`|The status placeholder displays the status of server|

### Gist of full URI

**To show number of online players**

`http://yourwebsite.com/apiv1/?get=js12sdk34ndk39fmpi3roijwr&show=onlineplayers`

**To show the status**, ***(Online, Maintenance, Offline)***

`http://yourwebsite.com/apiv1/?get=js12sdk34ndk39fmpi3roijwr&show=status`

##Script under build

The script is still undergoing development and needs to be finished. Please wait till then.

##Ideas

1 A complete web dashboard powerd by **SmartUCAPI** to show the status, players in your dashboard
2 Control the server using API (Done only via `POST` method with passowrd and IP recognition)
3 Encrypt data sent and recived through the RSA public and Private key (security)

# SMS Twillo Service

```
mesg-core service deploy https://github.com/emrekeskinmac/service-sms-twillo.git
```

## Tasks

### SendSms

#### inputs
| input | type | description |
| --- | --- | --- |
| accountSid | String | The Twillo Account SID that you can create here https://www.twilio.com/console |
| authToken | String | The Twillo Account Auth Token that you can create here https://www.twilio.com/console |
| from | String | The account to send the sms from |
| to | String | The recipient of the sms |
| body | String | The body of the sms |

#### outputs
| ouput | description |
| --- | --- |
| success | When the sms is successfully sent |
| failure | when an error occurs when trying to send the sms (this can be any kind of error, wrong phone number, Twillo API down...) |
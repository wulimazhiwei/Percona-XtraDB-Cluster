https://www.twilio.com/docs/notify/configure-ios-push-notifications#create-a-certificate-key


## sms push：
openssl pkcs12 -in MyApnsCert.p12 -out MyApnsCert.pem -nodes

voip push：
openssl pkcs12 -in MyApnsCert.p12 -nokeys -out cert.pem -nodes
openssl pkcs12 -in MyApnsCert.p12 -nocerts -out key.pem -nodes
openssl rsa -in key.pem -out key.pem

MyApnsCert.p12为p12文件名，MyApnsCert.pem为要生成的pem证书名称。
回车之后输入文件密码。

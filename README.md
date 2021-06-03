Remedyforce Ansible Example
=========

Getting a token
------------

```
curl -X POST -H "Content-Type: text/xml" -H 'SOAPAction: Login' --data-binary @login.xml https://202105240517350572.my.salesforce.com/services/Soap/u/35.0
```

XML File contents ....

```
<?xml version="1.0" encoding="utf-8" ?>
<env:Envelope xmlns:xsd=" http://www.w3.org/2001/XMLSchema "
    xmlns:xsi=" http://www.w3.org/2001/XMLSchema-instance "
    xmlns:env="http://schemas.xmlsoap.org/soap/envelope/">
  <env:Body>
    <n1:login xmlns:n1="urn:partner.soap.sforce.com">
      <n1:username>username</n1:username>
      <n1:password>password</n1:password>
    </n1:login>
  </env:Body>
</env:Envelope>
```

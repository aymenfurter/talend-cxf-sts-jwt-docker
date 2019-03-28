# talend-cxf-sts


	JWT Support:
	--------------------------------------
	Mar 28, 2019 8:45:59 PM org.apache.cxf.services.SecurityTokenService.UT_Port.STS
	INFO: Inbound Message
	----------------------------
	ID: 3
	Address: http://localhost:8080/UT?wsdl
	Encoding: UTF-8
	Http-Method: POST
	Content-Type: text/xml;charset=UTF-8
	Headers: {accept-encoding=[gzip,deflate], connection=[Keep-Alive], Content-Length=[1548], content-type=[text/xml;charset=UTF-8], host=[localhost:8080], SOAPAction=["http://docs.oasis-open.org/ws-sx/ws-trust/200512/RST/Issue"], user-agent=[Apache-HttpClient/4.1.1 (java 1.5)]}
	Payload: 
	<soapenv:Envelope xmlns:ns="http://docs.oasis-open.org/ws-sx/ws-trust/200512" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
		   <soapenv:Header>
	      <wsse:Security soapenv:mustUnderstand="1" xmlns:wsse="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd" xmlns:wsu="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd">
	         <wsse:UsernameToken wsu:Id="UsernameToken-F58F4572177B3478FC15537260095972">
	            <wsse:Username>tadmin</wsse:Username>
	            <wsse:Password Type="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-username-token-profile-1.0#PasswordText">tadmin</wsse:Password>
	
	         </wsse:UsernameToken>
	      </wsse:Security>
	   </soapenv:Header>
	   <soapenv:Body>
	      <wst:RequestSecurityToken Context="1aae57c8-092c-47a4-a5eb-c2ecbc21441d" xmlns:wsp="http://schemas.xmlsoap.org/ws/2004/09/policy" xmlns:wsp15="http://www.w3.org/ns/ws-policy" xmlns:wst="http://docs.oasis-open.org/ws-sx/ws-trust/200512" xmlns:wsu="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd">
        	 <wst:TokenType>urn:ietf:params:oauth:token-type:jwt</wst:TokenType>
	         <wst:RequestType>http://docs.oasis-open.org/ws-sx/ws-trust/200512/Issue</wst:RequestType>
	         <wst:Lifetime>
	            <wsu:Created>2013-09-17T18:18:10Z</wsu:Created>
	            <wsu:Expires>2013-09-17T18:23:10Z</wsu:Expires>
	         </wst:Lifetime>
	      </wst:RequestSecurityToken>
	   </soapenv:Body>
	</soapenv:Envelope>
	--------------------------------------
	Mar 28, 2019 8:45:59 PM org.apache.cxf.services.SecurityTokenService.UT_Port.STS
	INFO: Outbound Message
	---------------------------
	ID: 3
	Response-Code: 200
	Encoding: UTF-8
	Content-Type: text/xml
	Headers: {}
	Payload: 
	<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"><soap:Body><RequestSecurityTokenResponseCollection xmlns="http://docs.oasis-open.org/ws-sx/ws-trust/200512" xmlns:ns2="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd" xmlns:ns3="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd" xmlns:ns4="http://www.w3.org/2005/08/addressing" xmlns:ns5="http://docs.oasis-open.org/ws-sx/ws-trust/200802"><RequestSecurityTokenResponse Context="1aae57c8-092c-47a4-a5eb-c2ecbc21441d"><TokenType>urn:ietf:params:oauth:token-type:jwt</TokenType><RequestedSecurityToken><TokenWrapper xmlns:ns6="http://docs.oasis-open.org/ws-sx/ws-trust/200512" xmlns="">eyJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJ0YWRtaW4iLCJqdGkiOiJlMmI1NDZmZS1lZTBhLTQyNjEtOTYyOC01ZTI4NmVmZjllN2EiLCJpc3MiOiJEb3VibGVJdFNUU0lzc3VlciIsImlhdCI6MTU1MzgwNTk1OSwibmJmIjoxNTUzODA1OTU5LCJleHAiOjE1NTM4MDc3NTl9.mAv2JCo4SQN8MCbyznTjjEqSZYz67igMP2ND5pQZBEOGQhQoCkx_4f7f7hXDvTrZGL5ErVK1FBklaDjQfHVz_6x7iW20NzBIyeYwezHuMLs7yFtpTGQm7dTrPJArik83hqB1QPzVTjNrY-V1my53bheQ6E1OsQr6NIjlo6EWaAI</TokenWrapper></RequestedSecurityToken><RequestedAttachedReference><ns3:SecurityTokenReference><ns3:Reference URI="#e2b546fe-ee0a-4261-9628-5e286eff9e7a" ValueType="urn:ietf:params:oauth:token-type:jwt"/></ns3:SecurityTokenReference></RequestedAttachedReference><RequestedUnattachedReference><ns3:SecurityTokenReference><ns3:Reference URI="e2b546fe-ee0a-4261-9628-5e286eff9e7a" ValueType="urn:ietf:params:oauth:token-type:jwt"/></ns3:SecurityTokenReference></RequestedUnattachedReference><Lifetime><ns2:Created>2019-03-28T20:45:59.000Z</ns2:Created><ns2:Expires>2019-03-28T21:15:59.000Z</ns2:Expires></Lifetime></RequestSecurityTokenResponse></RequestSecurityTokenResponseCollection></soap:Body></soap:Envelope>
--------------------------------------

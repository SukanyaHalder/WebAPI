# WebAPI
Web API Interview Questions

<p style="line-height: 1;"><span style="font-size: 11px; font-family: &quot;Trebuchet MS&quot;, Helvetica, sans-serif;">Server Certificate vs Client Certificate</span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">How do we configure Server Certificate in WebAPI?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">How do we configure Cient Certificate in WebAPI?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">What is SslRequireCert?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">How do we see if a request is HTTP or HTTPs?&nbsp;</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">Why do we need SSL when we have basic authentication?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">How will we authenticate clients in Web API?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">How do you obtain SSL/TLS Certificate?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">What does SSL/TLS ensure?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">What is SSL?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">What are the types of SSL?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">What is SSL Handshake? How does SSL Work?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">What does SSL Certificate contain?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">SSL Heartbleed Vulnerability?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 
      11px;"><span style="font-family: 
        'Trebuchet MS', Helvetica, sans-serif;">What is Self Sign Certificate?</span></span></p>
<p style="line-height: 1;"><span style="font-size: 11px; font-family: &quot;Trebuchet MS&quot;, Helvetica, sans-serif;">How to install certificate on IIS?</span></p>
<p>
  <br>
</p><p>
  <br>
</p>
<p>Server Certificate vs Client Certificate</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Server Certificate authenticates server to clients</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Client certificate authenticates clietns to the server</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span></p>
<p>How do we configure Server Certificate in WebAPI?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- We install the certificate in IIS&nbsp;</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- WE create a AuthorizationFilter that checks whether the request is HTTP or HTTPS&nbsp;</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Apply the filter in Method in controller</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span></p>
<p>How do we configure Cient Certificate in WebAPI?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- two-way authentication</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- for better security</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- for eg in apps related to finance domain</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span></p>
<p>What is SslRequireCert?</p>
<p>
  <br>
</p>
<p>How do we see if a request is HTTP or HTTPs?&nbsp;</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Request.RequestUri.Scheme</p>
<p>
  <br>
</p>
<p>Why do we need SSL when we have basic authentication?&nbsp;</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- basic authentication sends everything in plaintext</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- it is not secure</p>
<p>
  <br>
</p>
<p>How will we authenticate clients in Web API?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- by issuing client certificates</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span></p>
<p>How do you obtain SSL/TLS Certificate?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- You purchase it from CA</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- You create self signed certificates for testing</p>
<p>
  <br>
</p>
<p>What does SSL/TLS ensure?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- integrity, authenticity and Encryption</p>
<p>
  <br>
</p>
<p>What is SSL?</p>
<p>&nbsp;- for establishing an encrypted link between a web server and a browser</p>
<p>&nbsp;- to ensure integrity, authenticity and Encryption</p>
<p>&nbsp;- SSL use port 443</p>
<p>&nbsp;</p>
<p>What are the types of SSL?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Extended Validation (EV) Certificates</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Organization Validated (OV) Certificates</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Domain Validated (DV) Certificates</p>
<p>
  <br>
</p>
<p>What is SSL Handshake? How does SSL Work?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Client (browser) sends hello to server giving him version of SSL it supports, cipher-suites it supports etc</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Server responds back with certificate and hello. Certificate contains the Public key.</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Client verifies the certificate by checking if it was authorized by CA</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Client sends a symmetric key encrypting it using the Public key sent by the server&nbsp;</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Server encrypts the data using the symmetric key (by decrypting</p>
<p>
  <br>
</p>
<p>What does SSL Certificate contain?</p>
<p>
  <br>
</p>
<p>SSL Heartbleed Vulnerability?</p>
<p>
  <br>
</p>
<p>What is Self Sign Certificate?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- a self-signed certificate is a certificate that is not signed by a certificate authority (CA)</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- These certificates are easy to make and do not cost money</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- people who visit that website will see a warning in their browser</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span></p>
<p>How to install certificate on IIS?</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Actual Certificate<span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span></p>
<p><span style="white-space:pre;">&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;</span>- IIS &gt; Certificate &gt; Complete Certificate Request &gt; Add certificate &amp; Save</p>
<p><span style="white-space:pre;">&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;</span>- Complete binding using https</p>
<p><span style="white-space:pre;">&nbsp; &nbsp;&nbsp;</span>- Self Signed Certificate</p>
<p><span style="white-space:pre;">&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;</span>- IIS &gt; Certificate &gt; Create Self Signed Certificate</p>

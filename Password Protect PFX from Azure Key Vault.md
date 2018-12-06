For some reason Azure Key Vault strips passwords from certificates, download them and use this code to password protect the private key:

```
$pfxBytes = [IO.File]::ReadAllBytes("/Users/alan/Downloads/xxx.pfx")
$pfx = New-Object Security.Cryptography.X509Certificates.X509Certificate2 -ArgumentList @($pfxBytes, "", [Security.Cryptography.X509Certificates.X509KeyStorageFlags]::Exportable)
$pfxProtectedBytes = $pfx.Export([Security.Cryptography.X509Certificates.X509ContentType]::Pkcs12, "b4zinga!")
[IO.File]::WriteAllBytes("/Users/alan/secure.pfx", $pfxProtectedBytes)
```

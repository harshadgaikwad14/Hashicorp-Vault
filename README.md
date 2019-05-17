# Hashicorp-Vault
 Managing Secrets using Hashicorp Vault.

# Window Installation
 YouTube : https://www.youtube.com/watch?v=HHEk4LDRpL0&list=PLZ8kCHLWBfBqovsXMMfR_BbM6ccs8x5Fc&index=4
 Download Hashicorp Vault : https://www.vaultproject.io/downloads.html
 Extract folder
 Run Command : D:\Harshad\Sowftware\vault_1.1.2_windows_amd64>vault.exe server -dev
 Web Url For Test : http://localhost:8200/
 ==> Vault server configuration:

             Api Address: http://127.0.0.1:8200
                     Cgo: disabled
         Cluster Address: https://127.0.0.1:8201
              Listener 1: tcp (addr: "127.0.0.1:8200", cluster address: "127.0.0.1:8201", max_request_duration: "1m30s", max_request_size: "33554432", tls: "disabled")
               Log Level: info
                   Mlock: supported: false, enabled: false
                 Storage: inmem
                 Version: Vault v1.1.2
             Version Sha: 0082501623c0b704b87b1fbc84c2d725994bac54

 WARNING! dev mode is enabled! In this mode, Vault runs entirely in-memory and starts unsealed with a single unseal key. The root token is already
 authenticated to the CLI, so you can immediately begin using Vault.

 You may need to set the following environment variable:

 PowerShell:
    $env:VAULT_ADDR="http://127.0.0.1:8200"
 cmd.exe:
    set VAULT_ADDR=http://127.0.0.1:8200

 The unseal key and root token are displayed below in case you want to seal/unseal the Vault or re-authenticate.

 Unseal Key: sWLzX7el5TBO+oyT1F0qkfAH5lUJs87350a3/pyDOrc=
 Root Token: s.pMAyBpFffDKweZsbn9vcw98R

 Development mode should NOT be used in production installations!
 
 
 D:\Harshad\Sowftware\vault_1.1.2_windows_amd64>set VAULT_ADDR=http://127.0.0.1:8200

 D:\Harshad\Sowftware\vault_1.1.2_windows_amd64>vault status
 Key             Value
 ---             -----
 Seal Type       shamir
 Initialized     true
 Sealed          false
 Total Shares    1
 Threshold       1
 Version         1.1.2
 Cluster Name    vault-cluster-22f354c5
 Cluster ID      32ec4823-5b00-09b4-a148-b34d55fa2642
 HA Enabled      false

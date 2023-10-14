# Cisco_Phone_Config
Config Cisco phone  7941 and 7942 XML file

**First Step:** Copy load files to the tftpboot Directory

## Cisco 7941 IP_Phone
> ~: cp SIP41.8-54S.loads /tftpboot/

## Cisco 7942 IP_Phone
> ~: cp SIP42.85-3S.loads /tftpboot/


**Second Step:** Copy the Config file to the tftpboot Directory and change the file

> ~: cp SEP(Cisco_IP_Phone_.7941_MAC).cnf /tftpboot/
> ~: cp SEP(Cisco_IP_Phone_.7942_MAC).cnf /tftpboot/
> ~: vi  **SEP(Cisco_IP_Phone_.7941_MAC).cnf** or **SEP(Cisco_IP_Phone_.7942_MAC).cnf**
Change the parts between ** according to the guide below

```mermaid
graph LR
A[**Your_NTP_Server_IP_Adress**] -- change to --> B[your server IP Address, for Ex: 192.168.1.100]
A[**Your_Server_IP_Adress**] -- change to --> B[your server IP Address, for Ex: 192.168.1.100]
A[**Phone_Label**] -- change to --> B[your Company name, for Ex: ParDevOPs]
A[****Extention_ID****] -- change to --> B[your Extention id, for Ex: 101]
A[****Extention_Pass****] -- change to --> B[your Extention Pass, for Ex: admin123]

```


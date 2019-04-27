# Instalar o filebeat


## linux

```
tar xzvf filebeat-7.0.0-linux-x86_64.tar.gz
```

## mac

```
tar xzvf filebeat-7.0.0-darwin-x86_64.tar.gz
```

## windows

1. Download the Filebeat Windows zip file from the downloads page.
2. Extract the contents of the zip file into C:\Program Files.
3. Rename the filebeat-<version>-windows directory to Filebeat.
4. Open a PowerShell prompt as an Administrator (right-click the PowerShell icon and select Run As Administrator).
5. From the PowerShell prompt, run the following commands to install Filebeat as a Windows service:

```
PS > cd 'C:\Program Files\Filebeat'
PS C:\Program Files\Filebeat> .\install-service-filebeat.ps1
```

Referência:
https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-installation.html

## Habilitar o módule `system`

    https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-module-system.html


Abrir os dashboards que foram criados no Kibana

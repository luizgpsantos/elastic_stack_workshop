# Instalar o metricbeat

## linux

```
tar xzvf metricbeat-7.0.0-linux-x86_64.tar.gz
```

## mac

```
tar xzvf metricbeat-7.0.0-darwin-x86_64.tar.gz
```

## windows

1. Extract the contents of the zip file into C:\Program Files.
2. Rename the metricbeat-<version>-windows` directory to Metricbeat.
3. Open a PowerShell prompt as an Administrator (right-click the PowerShell icon and select Run As Administrator).
4. From the PowerShell prompt, run the following commands to install Metricbeat as a Windows service:

```
PS > cd 'C:\Program Files\Metricbeat'
PS C:\Program Files\Metricbeat> .\install-service-metricbeat.ps1
```

Referência:
https://www.elastic.co/guide/en/beats/metricbeat/current/metricbeat-installation.html

## Habilitar o módulo `system`

O módulo `system` já vem habilitado por padrão. Basta verificar que dentro da pasta modules.d, seu nome seja `system.yml`.

- Criar os dashboards do Kibana

    https://www.elastic.co/guide/en/beats/metricbeat/current/load-kibana-dashboards.html

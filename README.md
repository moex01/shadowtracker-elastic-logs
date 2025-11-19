# ShadowTracker Logs
These are exported Elastic logs (in JSON format) of an end-to-end simulated ransomware attack scenario performed on a multi-machine environment. The purpose for sharing this publicly is to help DFIR professionals and SOC analysts to practice end-to-end investigations using Elastic SIEM and sharpen their skills through hands-on practice with real-world attack patterns and telemetry.

## Scenario
Contoso, a large technology company, has experienced a ransomware attack. As part of the incident response team, your task is to investigate the compromise and reconstruct the complete attack chain to ensure effective eradication and prevent the attackers from regaining access to the environment.


## Import into Elasticsearch Using elasticdump
You can import logs into your local Elastic instance by using the following example command:

```
elasticdump
--input=winlogbeat-*.json
--output=http://localhost:9200/<index_name>
--type=data
```

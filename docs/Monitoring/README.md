### Logstash

### ELK

### Prometheus

### Grafana

Шаблоны нотификаций
тест телеграмм

```
{{ .Status | toUpper }}{{ if gt (len .DashboardURL) 0 }}Dashboard: {{ .DashboardURL }}{{ end }}{{ if gt (len .Descriptions) 0 }}Description: {{ .Description }}{{ end }}
Value: {{ or .ValueString "[no value]" }}
```
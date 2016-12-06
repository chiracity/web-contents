+++
date = "2016-01-01T00:00:00-00:00"
title = "チラシティ"
+++
# チラシティ

<ul>
  {{ $sheetsId := "10o9Lz438Qg2V8pjhotQdXpJ-nUYclL20cpo6InTv7Wg" }}
  {{ $sheetsUrl := "https://docs.google.com/spreadsheets/d/" + $sheetsId +  "/export?format=csv&id=" + $sheetsId + "&gid=0"}}
  {{ $ad := getCSV $sheetsUrl }}
  {{ range first 5 $ad }}
      <li>{{ .pdf }} {{ .thumnail }} </li>
  {{ end }}
</ul>

## テスト

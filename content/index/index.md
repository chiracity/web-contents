+++
date = "2016-01-01T00:00:00-00:00"
title = "チラシティ"
+++
# チラシティ

{{ $sheetsId := "10o9Lz438Qg2V8pjhotQdXpJ-nUYclL20cpo6InTv7Wg" }}
{{ $sheetsUrl := "https://docs.google.com/spreadsheets/d/" + $sheetsId +  "/export?format=csv&id=" + $sheetsId + "&gid=0"}}
{{ $sep := "," }}
{{ range $i, $r := getCSV $sep $sheetsUrl }}
  <tr>
    <td>{{ index $r 0 }}</td>
    <td>{{ index $r 1 }}</td>
    <td>{{ index $r 2 }}</td>
  </tr>
{{ end }}


## テスト

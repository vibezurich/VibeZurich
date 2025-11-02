{{ define "main" }}
{{ range .Pages }}
- [{{ .Title }}]({{ .RelPermalink }})
{{ end }}
{{ end }}

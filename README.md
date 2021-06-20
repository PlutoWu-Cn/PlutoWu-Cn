# Hi there 👋

[![](https://img.shields.io/badge/blog-@PlutoWu-blue.svg)](https://plutowu.top)

```go
type resume struct {
	Name        string `info:"name" doc:"PlutoWu"`
	Sex         string `info:"sex"  doc:"Male"`
	Role        string `info:"role" doc:"SoftwareEngineer"`
	ChineseName string `info:"chineseName"  doc:"Shiyuan Wu"`
}

func findTag(str interface{}) {
	t := reflect.TypeOf(str).Elem()

	for i := 0; i < t.NumField(); i++ {
		taginfo := t.Field(i).Tag.Get("info")
		tagdoc := t.Field(i).Tag.Get("doc")
		fmt.Println("info:", taginfo, "doc:", tagdoc)
	}
}

func main() {
	var re resume

	findTag(&re)
}
```

## 🔧 Technologies & Tools

![](https://img.shields.io/badge/OS-Linux-orange.svg)
![](https://img.shields.io/badge/Editor-IDEA-green.svg)
![](https://img.shields.io/badge/Editor-GoLand-green.svg)
![](https://img.shields.io/badge/Language-Java-red.svg)
![](https://img.shields.io/badge/Language-GoLang-red.svg)
![](https://img.shields.io/badge/Language-JavaScript-white.svg)

## 📈 GitHub Stats

![PlutoWu's GitHub stats](https://github-readme-stats.vercel.app/api?username=PlutoWu-Cn&count_private=true&show_icons=true&theme=radical)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=PlutoWu-Cn&layout=compact&theme=radical&hide=html)

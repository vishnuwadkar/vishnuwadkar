package main

import (
	"fmt"
)

type Bio map[string]string

func main() {
	for k, v := range GetBio() {
		fmt.Printf("%+v: %+v\n", k, v)
	}
}

func GetBio() Bio {
	return Bio{
		"- ⚡ Quick bio:":                    "Living life on the edge of technology",
		"- 🔭 I’m currently studying in":      "Savitribai Phule Pune University",
		"- 🌱 I’m currently pursuing":        "Bachelor of Engineering in Artificial Intelligence and Datascience",
		"- 👯 I’m looking to collaborate on": "Python, C++, Web Development related projects",
		"- 🤔 I’m looking for help with":     "Anything related to what I am currently learning 😅",
		"- 💬 Ask me about":                  "Python, SQL, Software Design & Architecture, Web-Dev and SEO",
		"- 📫 How to reach me:":              "https://github.com/vishnuwadkar",
	}
}

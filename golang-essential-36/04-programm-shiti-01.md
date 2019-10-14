#  生命变量有几种方式?


```
package main

import (
	"flag"
	"fmt"
)

func main(){

	//方法一
	//var name string
	//flag.StringVar(&name,"name", "everyone", "The greeting object.")

	//方法二
	var name = *flag.String("name", "everyone", "The greeting object.")

	//方法三
	//name := *flag.String("name", "everyone", "The greeting object.")


	flag.Parse()

	fmt.Printf("Hello, %v!", name)


}
```






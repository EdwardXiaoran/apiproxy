

## 示例     
访问https://域名/https/api.openai.com/v1/chat/completions 
实际上会替换为https://api.openai.com/v1/chat/completions

如何在一些常见的开源项目中使用？
一般开源项目都是引用的openai的库，可以看到里面有一个属性是api_base = os.environ.get("OPENAI_API_BASE", "https://api.openai.com/v1")

所以使用的时候只需要设置一下openai.api_base="https://你的域名/https/api.openai.com/v1" 就可以了

映射规则为/https/url映射到https接口，/http/url映射到http接口


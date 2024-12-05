# 图片对比测试

## 单模型 convnext-large

### 目标图267kb 

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FgSCNuBihdL4wFvCXCZyDIKRumfk"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!60p"}],"models":["convnext-large"],"model_weights":[1],"similarity_method":"cosine"}
```

响应

```json
{"code":0,"message":"批量比对成功","similarities":[0.7281821,0.7226221,0.5580663,0.6712851],"success":true}
```

所有图片都没换存时耗时： 22920 ms

所有图片都有缓存时耗时： 1379 ms


### 目标图340kb 目标图变大，预设原图不变的情况下

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FjLJUt-aJsZ4Vibj8KT6nQm4_vhO"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!60p"}],"models":["convnext-large"],"model_weights":[1],"similarity_method":"cosine"}
```

响应

```json
{"code":0,"message":"批量比对成功","similarities":[0.7487665,0.7989278,0.5502855,0.747453],"success":true}
```

第一次 耗时 6873 ms

第二次  耗时 1566ms

### 目标图1Mb 目标图变大，预设原图不变的情况下

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/67457f7a47b7522f77d4d079/80920e331fc91f3983b631aba23acb65"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!60p"}],"models":["convnext-large"],"model_weights":[1],"similarity_method":"cosine"}
```

响应

```json
{"code":0,"message":"批量比对成功","similarities":[0.5846045,0.55593634,0.5591503,0.5586704],"success":true}
```

第一次 耗时 6882 ms

第二次  耗时 1515ms

### 目标图3Mb 目标图变大，预设原图不变的情况下

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/FvYhBvJLSYLZaxU7iXpXQyAbJHE2"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!60p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!60p"}],"models":["convnext-large"],"model_weights":[1],"similarity_method":"cosine"}
```

响应

```json
{"code":0,"message":"批量比对成功","similarities":[0.5846045,0.55593634,0.5591503,0.5586704],"success":true}
```

第一次 耗时 8259ms

第二次  耗时 1935ms

## 单模型 efficientnetv2-s

### 目标图267kb 

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FgSCNuBihdL4wFvCXCZyDIKRumfk"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!55p"}],"models":["efficientnetv2-s"],"model_weights":[1],"similarity_method":"cosine"}
```

响应

```json
{"code":0,"message":"批量比对成功","similarities":[0.67541677,0.7296374,0.59217215,0.7231734],"success":true}
```

第一次 耗时 10060ms (sources是全新图片)

第二次 耗时 1260ms

### 目标图340kb 目标图变大，预设原图不变的情况下

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FjLJUt-aJsZ4Vibj8KT6nQm4_vhO"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!55p"}],"models":["efficientnetv2-s"],"model_weights":[1],"similarity_method":"cosine"}
```

响应body

```json
{"code":0,"message":"批量比对成功","similarities":[0.673121,0.81757927,0.6459572,0.7305042],"success":true}
```

第一次 耗时 1523ms

第二次 耗时 1245ms

### 目标图1Mb 目标图变大，预设原图不变的情况下

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/67457f7a47b7522f77d4d079/80920e331fc91f3983b631aba23acb65"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!55p"}],"models":["efficientnetv2-s"],"model_weights":[1],"similarity_method":"cosine"}
```

响应body

```json
{"code":0,"message":"批量比对成功","similarities":[0.5315248,0.5558085,0.48591095,0.5358236],"success":true}
```

第一次 耗时 1557ms 

第二次 耗时 1239ms

### 目标图3Mb 目标图变大，预设原图不变的情况下

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/FvYhBvJLSYLZaxU7iXpXQyAbJHE2"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!55p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!55p"}],"models":["efficientnetv2-s"],"model_weights":[1],"similarity_method":"cosine"}
```

响应body

```json
{"code":0,"message":"批量比对成功","similarities":[0.57156694,0.57792485,0.7200957,0.55952984],"success":true}
```

第一次 耗时 2610ms
第二次 耗时 2434ms

## 双模型 efficientnetv2-s + clip-vit-base-patch16

### 目标图267kb 

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FgSCNuBihdL4wFvCXCZyDIKRumfk"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!52p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!52p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!52p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!52p"}],"models":["efficientnetv2-s","clip-vit-base-patch16"],"model_weights":[0.5,0.5],"similarity_method":"cosine"}
```

响应body

```json
{"code":0,"message":"批量比对成功","similarities":[0.39348197,0.41244245,0.36377916,0.41021323],"success":true}
```

第一次 耗时 9294ms

第二次 耗时 1510ms

### 目标图3MB 目标图变大，预设原图不变的情况下

请求body

```json
{"target":{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/FvYhBvJLSYLZaxU7iXpXQyAbJHE2"},"sources":[{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FsZW8OWb9xYHmRjlZcXKHczEKAJL?imageMogr2/thumbnail/!52p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FrFRY1MKUxlkyblf8tEYPV80MQn-?imageMogr2/thumbnail/!52p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/6749858057b01a6dbd81373f/Fv_Nr9ouiIFqEm8bQn3ofr4WHIBC?imageMogr2/thumbnail/!52p"},{"url":"https://cdn-qa-all.c360dn.com/travel-photography/resource/674816f414cc1927ac0352f1/FiyMM7zsVEXqZoB8tWqF1Ahzbgi_?imageMogr2/thumbnail/!52p"}],"models":["efficientnetv2-s","clip-vit-base-patch16"],"model_weights":[0.5,0.5],"similarity_method":"cosine"}
```

响应body

```json
{"code":0,"message":"批量比对成功","similarities":[0.3539229,0.35457158,0.41177243,0.35069],"success":true}
```

第一次 耗时 2823ms

第二次 耗时 2155ms
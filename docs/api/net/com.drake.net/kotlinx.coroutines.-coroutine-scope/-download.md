[net](../../index.md) / [com.drake.net](../index.md) / [kotlinx.coroutines.CoroutineScope](index.md) / [Download](./-download.md)

# Download

`fun CoroutineScope.Download(path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, dir: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = NetConfig.app.externalCacheDir!!.absolutePath, tag: `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`? = null, absolutePath: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)` = false, method: RequestMethod = RequestMethod.GET, uid: `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`? = coroutineContext[CoroutineExceptionHandler], block: Api.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)` = {}): Deferred<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>`

用于提交URL体下载文件(默认GET请求)

### Parameters

`path` - 请求路径, 非绝对路径会加上HOST[NetConfig.host](../-net-config/host.md)为前缀

`method` - 请求方式, 默认GET

`dir` - 下载文件存放目录 {默认存在android/data/packageName/cache目录}

`tag` - 可以传递对象给Request请求, 一般用于在拦截器/转换器中进行针对某个接口行为判断

`absolutePath` - 下载链接是否是绝对路径

`block` - 请求参数
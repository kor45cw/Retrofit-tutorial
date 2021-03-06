# Retrofit-tutorial

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fkor45cw%2FRetrofit-tutorial)](https://hits.seeyoufarm.com)

This is a sample project to show how to use Retrofit Libaray in your Android App.

- Java based
- use Android X 
- use databinding


## Used Libaray (사용한 라이브러리)

- [Retrofit](https://square.github.io/retrofit)
- [JSONPlaceholder](http://jsonplaceholder.typicode.com)

```groovy
dependencies {
    implementation 'com.squareup.retrofit2:retrofit:2.6.1'
    implementation 'com.squareup.retrofit2:converter-gson:2.6.1'
}
```

## Detail

1. MainActivity : just test Acitivty
2. RetroClient : create Retrofit instance and apiService. then networking 
3. RetroCallback : received data and pass UI thread
4. RetroBaseApiService : The api to access JSONPlaceholder
5. RequestPut : request form in put method
6. ResponseGet : received form in get method

NOTE

- Add Internet permission in AndroidManifest.xml
- (Android Q) add network_security_config.xml
```
<uses-permission android:name="android.permission.INTERNET"/>
```

## Output
![Output Image](https://raw.githubusercontent.com/kor45cw/Retrofit-tutorial/develop/output.png)

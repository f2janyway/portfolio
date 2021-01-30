# Portfolio

## 프로젝트

<pre>
<a href="https://play.google.com/store/apps/details?id=com.hyundaioilbank.android&hl=ko">
<img src="https://user-images.githubusercontent.com/55625423/106105029-a6fc5a00-6186-11eb-96ec-ab05c9881e5a.png" width="100"/>&nbsp오일뱅크 앱</a><br>
</pre>
- Kotlin
- 2020/06~2020/11 (6개월)
- coroutine, Retrofit2, Glide, Navigation-Component, Dagger2
- sns 로그인 연동, kicc pg결제 연동,  Zeplin, GoogleMap, git
- 오일뱅크 앱 리뉴얼로 안드로이드 앱(Kotlin)을 혼자 개발

<pre>
<a href="https://play.google.com/store/apps/details?id=com.box.bible&hl=ko">
<img src="https://user-images.githubusercontent.com/55625423/106109316-bbdbec00-618c-11eb-8597-c902ebc65135.png" width="100"/>&nbsp국한문성경 앱</a><br>
</pre>
- Java : Kotlin = 73 : 27
- 초기 개발 기간 10일 (19년 9월)
- 지금까지 계속 유지보수 및 업그레이드 중

<pre>
<a href="https://play.google.com/store/apps/details?id=com.box.firecast">
<img src="https://user-images.githubusercontent.com/55625423/106109559-08272c00-618d-11eb-8e73-561e76845eff.png" width="100"/>&nbsp멀티타이머 앱</a><br>
</pre>
-버전1 개발 기간 약 1주 (19년12월)
  - Java
-버전2 개발 기간 1주 (21년1월 중)
  - Kotlin
  
<pre>
<a href="https://play.google.com/store/apps/details?id=com.box.hymn&hl=ko">
<img src="https://user-images.githubusercontent.com/55625423/106109185-8fc06b00-618c-11eb-97e4-b917caeab559.png" width="100"/>&nbsp새찬송가 앱</a><br>
</pre>
- 개발기간 하루
- Kotlin

<pre>
<a href="https://github.com/yegyu/DotNet">
<img src="https://user-images.githubusercontent.com/55625423/106109942-723fd100-618d-11eb-9b28-7e94ff794e57.png" width="100" padding-left="10"/>&nbsp국비과정 프로젝트(웹 + 인공지능)</a><br>
</pre>
- 링크에 상세 있습니다.

<br>

- 블로그 : https://f2janyway.github.io/
- github : https://github.com/f2janyway<br>
- library: [link](https://github.com/f2janyway/custom_view)


## 취업후 경험 및 경력기술(20/2~20/11) 
 
### 첫 실무 프로젝트
- 오일뱅크 앱을 리뉴얼하는 업무(New-Project부터 시작했다.)
- 사수도 없이 지도하는 사람도 없이(PM분은 있었으나) 안드로이드 개발은 혼자했다.
- 안드로이드는 혼자 했지만 백엔드 개발자들과의 협업, 그리고 IOS개발자,기획자와의 의사소통을 통해 역시 소통이 참 중요함을 느꼈다.

## 유용한 코드
```kotlin
inline fun <T : OilDataInterface> callbackResult(
    call: Call<T>,
    crossinline remains: (Result<T>) -> Unit
) {
    call.enqueue(object : Callback<T> {
        override fun onFailure(call: Call<T>, t: Throwable) {
            remains(Result.Error(Exception(t.message)))
        }

        override fun onResponse(call: Call<T>, response: Response<T>) {

            if (response.isSuccessful) {
                if (response.body() == null) {
                    remains(Result.Empty)
                } else {
                    remains(Result.Success(response.body()!!))
                }
            } else
                remains(Result.Error(Exception("code : ${response.code()}")))
        }
    })
}
```
 
 ## 국한문 성경 
 
 ### 만든 이유
 1. 한자성경을 읽고 싶었으나 없어서<br>
 5000원 앱과 그냥 종이 한자 성경 스캔해 놓은것은 있었으나 사용하기 불편했음<br>
 사전 기능도 없음<br>
 
 ![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/b1_1.gif)
 <br>
 >ViewModel  + LiveData + RoomDatabase + Dao -> 간편 하이라이트 기능
 <br>

 ![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/b2.gif)
 <br>
 >기타 설정 기능 + 검색
 
 >알고리즘 사용
 >  > 검색어 색칠하기 
 >  > 검색어는 한글인데 한자가 포함되어 있기에 적용함
 <br>
 
 ![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/b3.gif)
 <br>
 >기본 기능
 
 <br>

<br><br>
## 멀티타이머
### 만든 이유
1. 구글 시계안의 타이머가 너무 불편해서
2. 왜 이런 타이머는 없을까 싶어서... 

![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/멀티타이머.gif)
 <br>

 
 ## 새찬송가

 ### 만든 이유
 1. 아빠가 만들어 달라고 하셔서
 


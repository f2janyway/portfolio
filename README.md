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
- 버전1 개발 기간 약 1주 (19년12월)
  - Java
- 버전2 개발 기간 1주 (21년1월 중)
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
- library : [link](https://github.com/f2janyway/custom_view)


<hr>

## 첫 실무 프로젝트
- 오일뱅크 앱을 리뉴얼하는 업무(New-Project부터 시작)
- 안드로이드는 혼자 했지만 백엔드 개발자들과의 협업, 그리고 IOS개발자, 기획자와의 의사소통을 통해 역시 소통이 참 중요함을 느낌.
<details>
  <summary>상세 기술</summary>
  
<br>  
  
* MVVM 구조와 AAC를 이용해서 개발을 진행했습니다.
* Navigation을 이용해서 기능(메인, 쿠폰, 지도 등등)별 Single Activity로 구현했습니다.
* 각 Activity에 기본적으로 Retrofit을 이용한 네트워크 통신이 있었기에 
* ViewModel이 하나씩 있었고 그 안에서 기능별 Repository를 나눠 나름대로 기능을 분류해 구현했습니다.
    * (EventRepository, StationRepository, UserRepository 등등 )
    
<br>

* ViewModel 안에서 MutableLiveData 를 private LiveData의 getter로 backing property 해주는 패턴으로 구현했습니다.
* 그리고 private val MutableLiveData를 repository 메서드에 파라미터로 넣어 
* repository에서 Retrofit2으로 response를 받아 파라미터에 setValue() 하여
* Activity or Fragment 에서 observe(Owner){} 방식으로 구현했습니다.

<br>

* dataBinding으로 view와 viewModel, activity, fragment를 연결하여 UI를 구성했습니다.

<br>

* 중복되는 xml의 경우 include를 이용해 중복을 줄였고 
* 그 view에서 databinding을 사용할 경우 @BindingAdapter을 이용해 분기하는 부분이 있었는데
* 해당 xml이 세 군데 이상일 경우는 복잡도가 증가해  
* @BindingAdapter 사용하지 않았습니다. 
* 사실 두 군데만 사용해도 추후 이해하는 데 어려움이 있어서 
* include 부분에서는 variable 변수명을 제대로 만들고 
* 나중에는  dataBinding을 사용하지 않는 방향으로 변경했습니다.

<br>

* retrofit enqueue를 제네릭으로 구현(아래 코드)하여
* Result 로 감싸고 View단에서 when 분기하여 각 응답을 처리하는 구조로 되었습니다.
* Retrofit Result(response.body) ->(Success, Error 등 분기하여)
* Repository ->
* ViewModel ->
* Activity or Fragment 에서 when(result){} 처리

<br>

* Dagger2을 이용해 ViewModel, Repository 등을 @Inject를 이용해 의존성 주입하였습니다. 

<br>

* MVVM 구조로 최대한 각 관심사를 분리하려 노력하였고
* 이런 구조로 되어있어 기능 추가 및 유지보수가 좀 수월함을 느꼈습니다.
* 정확히 기억은 안 나는데 대략 
* 8월 기본 앱 게시(이벤트, 지도, 멤버십결제 등등)
* 9월 회원가입, 회원정보수정 등 추가
* 11월 선결제, 주유 가격 등 추가 
* 이런 식으로 계속 업그레이드를 했는데 생각보다 어렵지 않았습니다. 

<br>

* 이미지 작업에서 제플린을 처음 사용해봤는데 
* shell을 이용해 이미지들이 각 사이즈별(hdpi,mdpi...) drawable에 넣어 편리하게 사용했습니다. 

<br>

* PG결제 모듈을 이용해 세차 멤버십이나 선결제 등 구현했습니다.
* 결제 기능은 웹뷰를 통해 구현 하였고 이는 거의 참고문서를 보고했습니다. 

<br>

* 영수증을 바코드로 찍어 누락 포인트 적립하는 기능이 있었는데
* Kicc모듈에서 계속 릴리즈 .apk로 실행하면 
* 버그가 나서 Crashlytics 로그를 보니 계속 Kicc 모듈에서 로그가 찍혀서
* '내 문제가 아니고 모듈문제'라고 계속 생각하다가 proguard 로 인해 모듈참조를 못 함을 알고
* -keep ~을 작성해서 문제를 해결했는데 
* 하마터면 계속 Kicc탓을 할 뻔했습니다.
* 이 경험을 통해 개발에 있어서 
* 항상 자신을 돌아봐야 함을 좀 크게 느꼈습니다.

<br>

* 첫 실무이고 혼자 하는 거라 걱정도 많이 있었고 어려운 점도 있었으나
* 생각보다 수월하게 진행이 돼서 ‘아 나도 충분히 할 수 있구나’라는 자신감을 얻는 계기가 되었습니다.

</details>


#### 프로젝트 속의 코드 
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
 
<details>
  <summary>기술 일부 상세</summarys>
  
<br>

* 한자와 한글이 적혀 있는 텍스트 파일(한자가 많이 미흡하고 오타도 많은)을 구해서
* 텍스트 파일을 Java로 `권`마다 나누고 또 각 `권`의 각 `장`으로 나누는 작업을 해서
* (성경.text -> 창세기/(1장, 2장...), 출애굽기/(1장, 2장…),...)의 형태로 나누고
* 또 각 `장`의 한자만 나누고 
* 그 한자들을 Python으로 크롤링 해서 한자의 이름과 뜻을 장마다 
* .txt 로 만들어서 
* 한자 사전용 파일을 만들어 일차적으로 기타 구현들을 하여 앱을 만들었습니다.

<br>

* 오타와 미흡한 한자가 많아서 
* 최대한 많은 1)`최대한 한자 수정을 한 파일`과 
* 다시 완전히 오타가 없는 2) `한글 성경 파일`을 크롤링해서 자료를 구하여 
* 2) 에다가 한글을 대조하여 한자를 집어넣는 작업을 수행했습니다.
* 이 알고리즘 작업에서 굉장히 머리를 많이 썼던 기억이 납니다.
* 이후에 오타는 전혀 없으나 한자를 넣는 작업 중
* 성경 전체를 완벽히 커버 하지는 못해서
* 여러 이용자의 도움을 받아 지금은 거의 빠진 한자나 오류 한자가 없습니다.(추정)

</details>
  
 
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
<details>
  <summary>기술 일부 상세</summary>
  
  <br>
  
* rx를 적용하고 TDD를 연습하려고 한 작업입니다.
* rxJava를 이용하지 않았고 Flow를 이용했습니다. 
* 또한, 간단한 커스텀 뷰가 들어가 있습니다. (CircleProgress)
* TDD원칙대로 테스트->구현을 순서대로 하진 못했습니다. 

<br>

* 각 타이머가 한 클래스를 이루고 
* View는 Presenter 방식으로 RecyclerView의 아이템으로 bind() 해주었습니다. 

<br>

* 리사이클러뷰 사용 시 
* 뷰를 재활용해서 여러 타이머를 만들고 
* recycle 할 때 뷰의 참조를 잘 맞추는 게 중요했습니다.
* (다시 해당 position에 와도 타이머가 진행 중이면 진행하고 있어야 하듯이)

<br>

* 알람 음을 사용하기 위해 contentsResolver를 이용해
* external 및 internal 음악, 벨소리를 query 해서
* uri를 구하고 알림을 구현했습니다. 

<br>

  </details>
  
<img src="https://github.com/yegyu/android_portfolio/blob/master/gif/멀티타이머.gif" width="280"/>
 <br>

 
 ## 새찬송가
 ### 만든 이유
 1. 아빠가 만들어 달라고 하셔서
<img src="https://github.com/yegyu/android_portfolio/blob/master/gif/hymn_gif.gif" width="280"/>
<br>
   
>터치바로 이뮬레이터를 실행한 화면이라 클릭이 좀 부자연스러움

<br>
 
 


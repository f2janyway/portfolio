# android_portfolio


### index
 - 개인앱,github 링크
 - 언어 , 안드로이드, 프로그래밍 level(?)
 1. 취업후 경험 및 경력기술<b>(20/11)</b>
 2. korean-chinese-Bible
 3. multi-timer
 4. 새찬송가
 5. (추가자료)인공지능 전문가 국비과정 프로젝트(19/4~19/10 7개월과정) [.Net](https://github.com/yegyu/DotNet)
    - 웹+리눅스+하둡+스파크 + 기타 하둡 에코시스템
    - 웹은 주도적으로 하나 나머지 머신러닝쪽은 따라하는 정도


## 개인 앱

<i>lean(?)하게 우선 빠르게 만들어 출시하고 버그로 호되게 혼나는 경험이 개발자로 많은것을 느끼게함...</i>

bible app link : https://play.google.com/store/apps/details?id=com.box.bible <br>
timer app lick : https://play.google.com/store/apps/details?id=com.box.firecast <br>
새찬송가 app link : https://play.google.com/store/apps/details?id=com.box.hymn&hl=ko <br>
github link : https://github.com/f2janyway<br>
첫 library: [link](https://github.com/f2janyway/custom_view)

## 20/11/16작성
주 언어:kotlin<br>
java > javascript > python> c++ > c(그냥 볼 줄은 알고 좀 사용할 수있는것들)<br>
linux,HTML,sql<br><br>
(익숙:레퍼런스 안보고는 다 할수 있는것은 아니나 많이 사용해서 익숙해진 정도;익숙하다고 제대로 아는것은 아님)<br>
(초보:자유자재로 하지는 못하고 좀 레퍼런스 보면서 구현 가능한)<br><br>

android(배움처는 거의 android관련 사이트 및 블로그)<br>

Android Components
- activities,fragments <- 익숙
- services <- 초보(일반적인 구현만 해봄,알람,notification,push연동)
- BroadCase Receivers <- 초보(일반적인 구현만 해봄,알람,notification,push연동)
- Content Providers <- 초보(많이 다뤄보지 않음)

Jetpack
- viewmodel, livedata, repository, room, navigation, dataBinding <- 익숙
- workmanager, paging3, cameraX  <- 초보

View
- cusstomview <- 초보
- constraintLayout <- 익숙
- MotionLayout <- 초보
- Transition,Animation <- 초보

API(경험)
- kakao,naver,google,apple login
- google-map
- kakao-navi, t-map
- pixabay

Library
- retrofit2, glide, zxing, socketIO, MPAChart

Gradle,(초보)
 - 알아서 한다기 보다는 거의 검색해서 필요한것 사용
Kicc모듈연동

Rx~ (많이 사용 안해봄;사실 안드로이드 개발하면서 크게 필요성을 못느꼈으나 현재 배워야할 필요는 느낌)<br>
Coroutine (초보와 익숙 사이)<br>
Flow or Sequence(초보와 익숙 사이)<br><br>

알고리즘(프래그래머스 level-2 간간히 푸는 정도)<br>
DS(기초는 있지 않나 생각하는데 모르는것 있으면 그때 그때 찾아봄)
 - 일반적인 개발에서 알고리즘보다 더 중요하다고 생각함


 
 ## 취업후 경험 및 경력기술(20/2~20/11) - 20/11/16작성
 ### - 20/2월 안드로이드로 첫 취업
 취업후 한달간 사수분의 과제를 하면서 `날코딩`을 한다는 말에 충격먹음.(절차지향,No 함수,No class)
 
 이후 최대한 쪼개보려고 함수로 나누고 또 공통 특징이 있는 함수들을 모아 클래스로 만드는 방식을 연습함.(from google codelab and android-developer site)
 
 지금껏 일하면서 구글에서처럼 의미단위로 다 쪼개진 않았지만(쉽지 않음) 충분히 필요성을 느낌.
 
 한달정도 과제하면서 레이아웃을 마음대로 짤수 있는 정도까지 습득을함. 사수분은 LinearLayout,RelativeLayout을 많이 사용하셨지만 ConstLayout을 주로 사용함.(물론 LinearLayout도 많이 사용하는데 RelativeLayout은 사용한적이 없음) 
 - ConstLayout의 장점은 뷰계층을 적게 해서 빠르고 효율적인(Google 曰) 리소스 사용을 한다고 해서 집착을 했는데 지금은 이 방식이 단순해서 매우 편리함.
 - 당시 AAC(안드로이드 아키텍쳐 컴포넌트)와 안드로이드 기본 지식들을 android develop 사이트에서 많이 읽고 (주로 AAC)실습 했음.
   - dagger (doc으로 잘 이해가 안갔으나 이 tutorial[youtube](https://www.youtube.com/watch?v=ZZ_qek0hGkM&list=PLrnPJCHvNZuA2ioi4soDZKz8euUQnJW65)을 보면서 이해함;상당히 유익)
   - navigaion-component (얘도 한번에 이해는 안됐는데 계속 따라해보고 반복하다보니 지금은 자연스럽게 어느정도 수월하게)
   - workmanager(몇번 읽고 대충 실습만 해본 정도-실전에선 적용해본적 없음)
   - viewModel-liveData-room 에 대해 많이 실습을 함.(처음에 기능분리를 하는 습관을 가지기에 좋은 선택이 viewModel이라고 느꼇음) 
   - testing은 doc을 봐도 android에서 가르쳐주는 udacity 영상으로도 실습하고 했지만 아직도 실전에 적용하기 버거움.(test필요성은 항상 느낌)
 - 코틀린 책(Kotlin in Action)을 보고 틈틈히 공부했다.(아직 단순 1회 독도 못하고 그냥 필요할때 찾아보고 있다.) 
 
이때가 실력이 두번째로 많이 오른 타이밍이었던것 같다.(처음은 국비과정 중간)

이 후에 몇몇 앱의 유지보수를 맡았고 실상 애플로그인추가한것 외엔 딱히 한게 없다.

### 첫 SI 프로젝트(지금에는 정말 값진 경험)
[H 정유사 앱 링크](https://play.google.com/store/apps/details?id=com.hyundaioilbank.android&hl=ko)(11/30 마지막 오픈)

#### 대략 설명 및 느낀점
- H 정유회사의 앱을 리뉴얼하는 업무(New-Project부터 시작했다.)
- 사수도 없이 지도하는 사람도 없이(PM분은 있었으나) 안드로이드 개발은 혼자했다.
- 처음에는 그 대기업의 앱을 나 혼자 만들어야한다는 중압감이 엄청 스트레스였는데 사수분은 계속 넌 할수 있으니 걱정말라고 말을 많이 해주었다.그래도 당시에는 스트레스가 심했다.
- 대기업이어서 그런지 아니면 관련 사람이 많아서 그런지 개인적으로 일하는 스타일이 많이 안맞는다는것을 애초에 느꼈다. 
- 안드로이드는 혼자 했지만 백엔드 개발자들과의 협업, 그리고 IOS개발자,기획자와의 의사소통을 통해 역시 소통이 참 중요함을 느꼈다.
- 리뷰폭격으로 스트레스 받는 파견자와 별 미동도 없는 주인들... 이점이 마음에 안들었다.

#### 코딩관련
* 제플린을 이용하는데 이미지파일을 다운 받고 .zip 파일 풀고 res/drawable에 넣고 하는 작업이 귀찮을게 뻔해  unzip script를 만들어 지금껏 시간을 많이 아꼈다.
* 처음에 설계를 잘짜놔야 한다는 생각에 파견가기 전에 viewMdoel,dataBinding 을 제네릭으로 하는 추상 BaseActivity,BaseFragment,BaseActivityNoViewModel 등을 공부하고 구현해 두었다.
* 네트워크 통신(비동기로)을 많이 하기에 retrofit2도 lamda,generic으로 inline function을 만들어 놨다.(이거 만들때 고차함수에 대해 좀 익숙하게 되었다.)
  * 이 activity, retrofit, fragment 들을 generic 으로 만들어 놓고 하니 시간과 코드가 많이 단축됨을 느끼고 개발했다.(아마 더 좋은 설계가 있겠지만 나로는 잘한 시도였다.)
```kotlin
//이게 정말 좋은 코드인지는 정확히 모르겠다...inline은 객체생성의 overhead를 막고 crossinline으로 또 인자를 받을수 있는 함수를 사용하기에 편리는 한데
//이게 정말 성능이 좋은지는 모르겠다. profiler나 디컴파일해서 소스,성능 분석하는 단계가 되진 못했다.
inline fun <T : OilDataInterface> retrofitCallback(
    call: Call<T>,
    con:Context? = null,
    crossinline remains: (T) -> Unit
) {
    call.enqueue(object : Callback<T> {
        override fun onFailure(call: Call<T>, t: Throwable) {
            con?.let { toast(context = it, msg = it.getString(R.string.network_fail)) }
        }

        override fun onResponse(call: Call<T>, response: Response<T>) {
            val data = response.body()
            if (data != null)
                remains(data)
        }
    })
}
```
* 입사 후 공부해놓은 dagger와 navigation으로 도움을 많이 받았다.
  * dagger을 이용해 Repository,SnsLogin 를 inject해서 여러군데서 간편히 적용을 시킬수 있었다.(사실 dagger는 사용해보고 싶어서 사용했다.)
  * navigation도 2차 부터(거의 중간) 도입을 시작했다. 맨처음엔 홈화면을 다 BottomNavigationView 와 fragment들도 연결시켜서 각각으 로직을 다 구현했는데 2차 땐 회원가입이 있어서 거기에 navigation을 도입해(이때쯤 적용해볼수 있겠다 싶었다.)덕분에 회원가입 Flow를 간편히 짤 수 있었다. 그리고 이후 fragment가 들어가는 부분에 많이 적용하고 홈화면에도 다시 적용을 했다.
  * 이 navigation을 유일하게 다시 supportFragmentManager를 이용해 변경한 부분이 있었는데 누락포인트 적립이라고 카메라로 바코드 찍어 적립하는 곳이었는데 이상하게 삼성의 몇몇 폰(안드로이드 10)에서 바코드 인식후(onActivityResult) navigate() 후에 white(blank)screen이 되는 현상이 있었다. 이것 때문에 구글링도 하고 해서 livedata.observe()가 여러번 observe를해서 그 안에서 navigate()가 여러번 되서 그런현상이 있다는 글이 있어서 그것도 다시 그냥 call.enqueue로 해봤지만 같은 현상이 있었다. 시간이 없어 그냥 navigation을 포기했는데 시간이 나면 꼭좀 해결해보고 싶다.(삼성폰의 문제또는 아드로이드10과의 충돌인 버그라고 짐작도 들지만...)
  * 
* 많은 수정사항들을 수정하면서 객체 지향과 코드의 (기능별)함수화가 얼마나 잘 되어 있느냐 또 코드가 얼마나 깔끔하냐가 중요함을 느꼈다. 생각보다 거의다 금방금방 해결했다.
* 서버통신에선 전부 request(POST)를 하는 형태고 tomcat 서버에 spring을 사용했는데 처음에 국비과정에서 프로젝트를 재미있게 했던 것들이 백엔드 개발자들과의 소통에 많은 도움이 됐다.(도움도 주고)
* retrofit에서 에러핸들링이 많이 미흡함을 느꼈다.(sealed class를 만들어서 하는게 좋은데...)
* 여기는 테스트/빌드 자동화같은게 없어서 (낮에)필요하면 운영기를 새로고침하고 했는데 이로인해 리뷰의 빨간 줄들이 많이 생겼다. 안드로이드 개발할때도 테스트의 필요성은 느끼는데 이를 구현해놓기가 참 힘들었다. 우선 테스트 하기 좋은 코드가 아니었던게 첫 문제였던것 같다. 그리고 보통은 UI와 하드웨어와 서버를 테스트해야하는데 이걸 어떻게 해야하나 하면서 그냥 테스트를 직접 손으로 눈으로 했는데 이 시간이 정말 아까웠다.
* 지도에서 주유소 마커에 나인패치 이미지를 놓고 또 지도를 줌 아웃하면 급 느려지는 현상이 있었는데 여기선 일정 zoom이면 그냥 클러스터 되게했다. 여기서 ClusterManger,ClusterManagerRenderer을 커스텀하면서 좀 느려지는 부분(이미지 전환)을 해결했다. 언젠가부터 느끼는 거지만 커스텀을 잘하는것과 직접구현을 할 수 있는 능력이 중요한것 같다. clusterManager을 addItems()를 할 때 나름 알고리즘을 짜서 좀 효율적으로 해보려 했으나 그것보다 clustermanager에서 알아서 캐쉬해줘서 전체 remove() 후 addItems()를 하는게 더 좋았는데 모르겠다. 내 알고리즘 실력이 부족했을 이유가 좀 컸다고 생각한다.(괜히 알고리즘 알고리즘 하는게 아니다.)
* 요번에 바코드 인식에 zxing라이브러리를 사용했는데 인식이 잘 안된다는 고객의 컴플레인이 있었다. 그러면서 몇몇 어플과 MKKit를 사용한 앱을 다운받고 시도를 해봤는데 결론은 해당 바코드는 어디서든 잘 안찍혔다.(길기도 하고 흐리기도 하고 배경이 흰색이 아니고 다른 색의 글자들도 있고)그런데 그나마 mlkit를 사용한 것들은 좀 빨리 인식이됐다. 그래서 당장에 이걸 프로젝트에 적용은 못하지만 CameraX와 MLKit를 이용해 구현해 봤는데 처음 레퍼런스도 많이 없고 해서 좀 헤맸는데 구현하고 보니 별거 없었다. 이 역시 회사의 바코드는 잘 인식을 못했다.(내장 테스트,훈련(?)파일을 이용) 아마 구글 클라우드를 사용하는건 인식이 좀더 잘되지 않을까 싶다.


 
 ## 국한문 성경 
 * 언어 : <b>Java</b>-><b>Java : Kotlin = 9 : 1</b>-> 현재<b>Java : Kotlin = 7.5 : 2.5</b> 
 * (20/1/28~) ViewModel + LiveData + Room (하이라이트 부분) 
 * (20/9/1~) Repository 추가(Room, SharedPreference)
 * <b>(20/11)</b> 검색쪽(just contains()만 사용)에 fastscroll용으로 customLayout을 만들고 라이브러리를 만듬 [library](https://github.com/f2janyway/custom_view/blob/master/f2j_custom_view/src/main/java/com/box/f2j_custom_view/VerticalSeekBar.kt)
  - VerticalSeekbar로 만들고 싶었으나 View size에 따라 thumb 위치를 못 맞춰 Seekbar는 못됨
 
 ### 만든 이유
 (20/1 작성)
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
 ### 기타 설명
(20/1월중 작성)
* 액티비티 수: 4 
* 프래그먼트 수 : 2 ( in viewpager2 )
* 초기 개발 시간 : 안드로이드 처음 시작한 이후 10일(대략) 19/9/11-21 ( java )
* 추가 기능 더한 순서 : 
  - 계속 읽기 책갈피 기능(SQLite) 
  - 메인화면(제목들) : 리스트뷰-> 리사이클러뷰 -> view pager2 (첫번째 gif)
  - 검색어 표시 (두번째 gif)
  - 하이라이트 기능 (첫번째 gif) : 이때 코틀린 적용 (java + 코틀린)
  - 검색 페이지에 fastScroll 커스텀

* 최대한 사용자가 편하고 유용하게 사용하기를 바라는 마음으로 기능 구현함.
## 프로그래밍적
* 한자만 또는 한글만 또는 한자(한글) 또는 한글(한자)의 형식을 짜는 코드를 짜면서 머리를 꾀 사용함.
* 성경 전체의 한글 오타나 (빠진 한문들도) 문장이 원문과 다른 것들을 고치는 코딩을 하면서 알고리즘(시간복잡도,공간복잡도를 전혀 신경쓰지 않은)이라긴 모해도 전적으로 당장의 문제를 해결하기 위해 머리를 많이 써야했음.
* 사용자들의 요구사항들을 반영하면서 유지보수성이 좋은 코드의 필요성을 많이 느낌(지금에서도 사실 손대기 무서울 정도의 코드로 되어있음)
* firebase 및 Crashlytics 연동
* 현재 800명 이상 다운로드->현재<b>(20/11)</b> 5천 이상(google console에서 프러덕트 수는 4000명대)
* 한자 사전 기능
* 전부 txt 파일로 불러옴, 데이터 사용 없음(firebase,Crashlytics 제외)
* 유용하게 쓰여서 기분 좋음(from review)

<br><br>
## 멀티타이머
 * 언어 : <b>코틀린</b> 
 * Activity + Service + BroadCastReceiver
### 만든 이유
1. 구글 시계안의 타이머가 너무 불편해서
2. 왜 이런 타이머는 없을까 싶어서... 
3. 쓰레드 공부 하려고
4. Service & BroadCastReceiver 사용해 보려고

![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/멀티타이머.gif)
 <br>
![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/멀티타이머2.gif)
 
 ### 기타 설명
 * 액티비티 수 : 1 
 * 개발 기간 : 7 일 (대략)19/12/2-9 
 * 사용자수 한명... 저...
   - 일반적으로 사람들이 타이머를 잘 사용안하는 것 같음
   - 구글 어시스턴트가 훨씬 편함...
 * notification 공부를 하게 됨
 * mediaplayer 적용(해당 벨소리로만)
 * vm + livedata + coroutine을 사용하기 적합한 앱
    - 사용자가 있으면 바꿔보고 싶은데 사실 동기 부족...
 * admob 적용 
    - 이것도 신중해야할 것 같음
 
 * 의욕적으로 언어도 한 40개국을 적용했으나 번역 프로그램만 만듬...
    - 파이썬 셀레늄으로 구글 번역기로 돌려서 여러나라 언어를 뽑음
    - 구글 스토어에 올릴 때 , 업데이트할 때 용도로 
 * <b>(20/11)</b> 구글 타이머와 비슷하게 원(circle)형 progressbar(seekbar)로 만들어 보려고 customlayout 만들어봄 [library](https://github.com/f2janyway/custom_view/blob/master/f2j_custom_view/src/main/java/com/box/f2j_custom_view/CircleProgress.kt)
 * 아직까지<b>(20/11)</b>이것저것 할게 있어서 손을 못대고 있음.-
 * Thread와 Timer을 사용함. coroutine은 거의 사용안함.
 
 ## 새찬송가
 * 코틀린(100%)
 * [code](https://github.com/f2janyway/hymn/tree/master/app/src/main/java/com/box/hymn)
 ### 만든 이유
 1. 아빠가 만들어달라고 해서
 
 - 제작기간(8월달 언젠가 하루)
 - 위의 개인 앱들 중에 가장 최근에 만들거라 코드가 그나마 깔끔하다.(물론 내용도 별거 없고 빨리 그냥  앱이지만)
 - 항상 느끼는 거지만 의미(or 기능) 단위로 패키지화하는 것도 쉽지 않음을 느낀다.
 
 
 
 
 
 
 
## Android Study
* 주 공부처 : Android Developer 문서 및 codelabs.developers 그리고 구글 코드 기타 블로그 등등


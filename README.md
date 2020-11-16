# android_portfolio
## 개인 앱
bible app link : https://play.google.com/store/apps/details?id=com.box.bible <br>
timer app lick : https://play.google.com/store/apps/details?id=com.box.firecast <br>
새찬송가 app link : https://play.google.com/store/apps/details?id=com.box.hymn&hl=ko <br>
gitHub link : https://github.com/f2janyway
### index
 1. 취업후 경험 및 경력기술<b>(20/11)</b>
 2. bible
 3. multi-timer
 4. 새찬송가
 5. (추가자료)국비과정 프로젝트(19/4~19/10 7개월과정) [.Net](https://github.com/yegyu/DotNet)
 
 ## 취업후 경험 및 경력기술(20/2~20/11) - 20/11/16작성
 - 20/2월 안드로이드로 첫 취업
 취업후 한달간 사수분의 과제를 하면서 날코딩을 한다는 말에 충격먹음(절차지향,No 함수,No class)
 
 이후 최대한 쪼개보려고 함수로 나누고 또 공통 특징이 있는 함수들을 모아 클래스로 만드는 방식을 연습함(from google codelab and android-developer site)
 
 지금껏 일하면서 구글에서처럼 의미단위로 다 쪼개진 않았지만(쉽지 않음) 충분히 필요성을 느낌
 
 한달정도 과제하면서 레이아웃을 마음대로 짤수 있는 정도까지 습득을함. 사수분은 LinearLayout,RelativeLayout을 많이 사용하셨지만 ConstLayout을 주로 사용함(물론 LinearLayout도 많이 사용하는데 RelativeLayout은 사용한적이 없음) 
 - ConstLayout의 장점은 뷰계층을 적게 해서 빠르고 효율적인(Google 曰) 리소스 사용을 한다고 해서 집착을 했는데 지금은 이 방식이 단순해서 매우 편리함.
 
 
 
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

* 최대한 사용자가 편하고 유용하게 사용하기를 바라는 마음으로 기능 구현함
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
 * mvvm + livedata + coroutine을 사용하기 적합한 앱
    - 사용자가 있으면 바꿔보고 싶은데 사실 동기 부족...
 * admob 적용 
    - 이것도 신중해야할 것 같음
 
 * 의욕적으로 언어도 한 40개국을 적용했으나 번역 프로그램만 만듬...
    - 파이썬 셀레늄으로 구글 번역기로 돌려서 여러나라 언어를 뽑음
    - 구글 스토어에 올릴 때 , 업데이트할 때 용도로 
 * <b>(20/11)</b> 구글 타이머와 비슷하게 원(circle)형 progressbar(seekbar)로 만들어 보려고 customlayout 만들어봄 [library](https://github.com/f2janyway/custom_view/blob/master/f2j_custom_view/src/main/java/com/box/f2j_custom_view/CircleProgress.kt)
 
## Android Study
(20/1)
* 주 공부처 : Android Developer 문서 및 codelabs.developers 그리고 구글 코드 기타 블로그 등등
* viewModel (livedata ) + repository (retrofit2, room) 구조를 구글에서 알려주는데 그 효용을 느낌. Test는 잘 못하지만 유지보수성에 편리함 
* dagger (오일뱅크 프로젝트에 적용)
* Test 연습이 많이 필요
    - JUnit assertThat, assertEqual 은 사용 해봄
    - instrument test는 아직 해보지 않음 (espresso 등등)



# android_portfolio

bible app link : https://play.google.com/store/apps/details?id=com.box.bible <br>
timer app lick : https://play.google.com/store/apps/details?id=com.box.firecast

### index
 1. bible
 2. multi-timer
 3. studied
 
 ## 국한문 성경 
 * 언어 : <b>자바 : 코틀린 = 8 : 2</b> 
 ### 만든 이유
 1. 한자성경을 읽고 싶었으나 없어서<br>
 5000원 앱과 그냥 종이 한자 성경 스캔해 놓은것은 있었으나 사용하기 불편했음<br>
 사전 기능도 없음<br>
 
 ![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/b1.gif)
 <br>
 >RoomDatabase + Dao -> 간편 하이라이트 기능
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

* 액티비티 수: 4
* 프래그먼트 수 : 2 ( in viewpager2 )
* 초기 개발 시간 : 안드로이드 처음 시작한 이후 10일 ( java )
* 추가 기능 더한 순서 : 
  - 계속 읽기 책갈피 기능(SQLite) 
  - 메인화면(제목들) : 리스트뷰-> 리사이클러뷰 -> view pager2 (첫번째 gif)
  - 검색어 표시 (두번째 gif)
  - 하이라이트 기능 (첫번째 gif) : 이때 코틀린 적용 (java + 코틀린)

* 최대한 사용자가 편하고 유용하게 사용하기를 바라는 마음으로 기능 구현함
* firebase 및 Crashlytics 연동
* 현재 800명 이상 다운로드
* 한자 사전 기능
* 전부 txt 파일로 불러옴, 데이터 사용 없음(firebase,Crashlytics 제외)

<br><br>
## 멀티타이머
 * 언어 : <b>코틀린</b> 
### 만든 이유
1. 구글 시계안의 타이머가 너무 불편해서
2. 왜 이런 타이머는 없을까 싶어서... 
3. 쓰레드 공부 하려고

![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/멀티타이머.gif)
 <br>
![Alt Text](https://github.com/yegyu/android_portfolio/blob/master/gif/멀티타이머2.gif)
 
 ### 기타 설명
 * 액티비티 수 : 1 
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
 
## Android Study
* 주 공부처 : Android Developer 문서 및 codelabs.developers 그리고 구글 코드 기타 블로그 등등
* mvvm + room + livedata 아직 익숙하지는 않으나 구현 가능
* dagger (DI + Ioc) 익숙하지 않으나 문서를 쭉 봐본 결과 스프링과 매우 유사함을 느낌
* Test 역시 익숙하지 않으나 연습이 많이 필요할 것 같음
    - Junit assertThat, assertEqual 은 사용 해봄
    - instrument test는 아직 해보지 않음 (espresso 등등)

<br><br><br>

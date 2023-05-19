## 반응형 웹 페이지
### 감지된 화면 크기에 따라 자동으로 페이지가 재배열되는 유동적인 접근 방식이다.
- CSS 미디어 쿼리(맞춤형 스타일 시트)를 사용하여 최종 사용자가 사용하는 기기의 특성을 검사한다.
- 그 후 웹사이트에서 검사된 내용을 바탕으로 자체적으로 렌더링된다.

반응형 웹을 정확히 이해하기 위해서는 **적응형 웹**이 무엇인지도 파악해야할 것 같아 가져왔다.

#### [적응형 웹]은 웹 페이지에서 감지된 기기를 기반으로 미리 만들어진 정적인 레이아웃을 불러오는 방식이다.
- 디자이너가 다양한 화면 너비에 맞춰 별도로 디자인 작업을 해야한다.
- 가장 일반적인 너비는 다음과 같다. (단위:픽셀)
    - 320
    - 480
    - 760
    - 960
    - 1200
    - 1600
- `애플`이 적응형 디자인을 사용한 좋은 예시다.

즉, 반응형 디자인과 적응형 디자인의 장단점은 다음과 같다. (출처:[wixblog](https://ko.wix.com/blog/post/responsive-vs-adaptive-design))
```bash
# 반응형 디자인
 장점 - 모든 플랫폼에서 일관된 콘텐츠 경험
     - 보편적이지 않은 화면 크기의 새로운 기기에서도 작동 가능
 단점 - 각 기기에서 웹사이트가 렌더링되는 방식에 대한 통제가 상대적으로 어려움
     - 요소가 잘못된 순서 또는 크기로 재배치되는 경우 시각적 계층 구조를 방해함
     - 디자인에 대한 더 많은 전문 지식이 필요함. 플랫폼 간 테스트 및 디자인 조정을 요함
     - 동적 콘텐츠를 불러오는 데 더 많은 작업이 요구되어 웹사이트 성능이 저하됨

# 적응형 디자인
 장점 - 각 플랫폼 및 상황과 맥락에 맞춰 제공되는 완벽한 맞춤화된 경험
     - 원하는 기기에 맞게 최적화된 디자인을 할 수 있는 고성능 작업 수행
     - 광고 및 타사의 통합 콘텐츠에 대한 간편한 맞춤화
 단점 - 콘텐츠가 모든 기기에서 일관되지 않을 경우 `SEO`에 부정적인 영향을 미침
```
* 여기서 SEO란?
  - Search Engine OPtimization의 줄임말
  - 검색 엔진 최적화 = 검색 결과에서의 상위 노출을 의미.
    즉, SEO를 한다는 의미는 '검색 엔진이 정한 상위 노출을 위한 조건을 맞춰 나가는 과정'이다.

## 반응형 웹 페이지를 구현하기 위해 알아야 할 것들
### 미디어 쿼리
- CSS Media Queries
    - 미디어 쿼리는 CSS2부터 시작되어 CSS3에서 본격적으로 쓰이기 시작한 웹 기법이다.
    - 디바이스의 폭이나 높이 등의 정보를 가지고 스타일을 개별적으로 줄 수 있다.
    - 예문
    ```css
    @media 미디어 타입 (너비 및 높이) {
        (CSS 입력)
    }       
    ```
    > 반응형 웹은 보통 HTML, CSS로 구현이 가능하지만, 불가능한 것들도 있다.

### 뷰포트 설정
- 뷰포트(Viewport)란 `모니터의 출력에 대한 화면 영역을 설정하는 것`이다.
- 뷰포트를 명시하지 않을 경우, 반응형으로 웹 디자인을 작업하더라도 PC 화면이 떠버리는 결과가 발생한다.

   **뷰포트 명시법**
    - HTML의 <meta> 태그 이용하기; Safari에서 처음 사용하여 크롬, 오페라, 파이어폭스 등으로 따라서 적용한 방식이다.
    - CSS에서 직접 명시; W3C에서 권장하는 방식, 표준화가 완전히 되지 않아 `IE10`이상과 `오페라`에서만 지원하고 있다.

### 특징
1) 하나의 코드
    - 하나의 콘텐츠에 오직 하나의 HTML 소스만 존재한다.
    - 특정 장치에 최적화된 여러가지의 HTML이 있으면 반응형 웹이라고 부르지 않는다.
  (CSS, JS 파일은 여러가지가 존재할 수 있음)
2) 하나의 URL
    - 특정 장치에 최적화된 페이지로 연결되는 별도의 URL이 있으면 반응형 웹이라고 부르지 않는다.

## 반응형 웹 페이지 - 예시 사이트
- [토요타](https://www.toyota.co.kr/)
    #### 다음은 나무위키 검색 결과에서 가져온 사이트들이다.
<ul class="U2I+aqnk" data-v-d9583359=""><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/Daum" title="Daum" data-v-d9583359="">Daum 어학사전</a> <a class="QuDd1Dh0" href="http://alldic.daum.net/" target="_blank" rel="nofollow noopener" title="http://alldic.daum.net/" data-v-d9583359="">#</a><a class="yDQWz7wG" href="#fn-4" data-v-d9583359=""><span id="rfn-4" data-v-d9583359=""></span>[4]</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/plug.dj" title="plug.dj" data-v-d9583359="">plug.dj</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EA%B8%B0%EA%B8%80%ED%95%98%EB%93%9C%EC%9B%A8%EC%96%B4" title="기글하드웨어" data-v-d9583359="">기글하드웨어</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><strong data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EB%82%98%EB%AC%B4%EC%9C%84%ED%82%A4" title="나무위키" data-v-d9583359="">나무위키</a></strong><a class="yDQWz7wG" href="#fn-5" data-v-d9583359=""><span id="rfn-5" data-v-d9583359=""></span>[5]</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EB%88%88%EB%88%84" title="눈누" data-v-d9583359="">눈누</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EB%8B%88%EC%BD%98" title="니콘" data-v-d9583359="">니콘</a> <a class="QuDd1Dh0" href="http://www.nikon-image.co.kr" target="_blank" rel="nofollow noopener" title="http://www.nikon-image.co.kr" data-v-d9583359="">#</a> - <a class="sl8O8g9f" href="/w/2016%EB%85%84" title="2016년" data-v-d9583359="">2016년</a> <a class="sl8O8g9f" href="/w/7%EC%9B%94%205%EC%9D%BC" title="7월 5일" data-v-d9583359="">7월 5일</a>부터 홈페이지를 개편하면서 기존 PC 전용 페이지에서 반응형 웹 디자인을 적용시켰다.</div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EB%8F%84%EC%BF%A0%EC%9C%84%ED%82%A4" title="도쿠위키" data-v-d9583359="">도쿠위키</a> 사이트 다수<a class="yDQWz7wG" href="#fn-6" data-v-d9583359=""><span id="rfn-6" data-v-d9583359=""></span>[6]</a><a class="yDQWz7wG" href="#fn-7" data-v-d9583359=""><span id="rfn-7" data-v-d9583359=""></span>[7]</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EB%8F%99%ED%83%84%EA%B3%A0%EB%93%B1%ED%95%99%EA%B5%90" title="동탄고등학교" data-v-d9583359="">동탄고등학교</a> <a class="QuDd1Dh0" href="http://dongtan.hs.kr" target="_blank" rel="nofollow noopener" title="http://dongtan.hs.kr" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EB%B3%91%EB%AC%B4%EC%B2%AD" title="병무청" data-v-d9583359="">병무청</a> <a class="QuDd1Dh0" href="http://www.mma.go.kr" target="_blank" rel="nofollow noopener" title="http://www.mma.go.kr" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EC%84%9C%EB%8B%B4(%EC%9B%B9%EC%82%AC%EC%9D%B4%ED%8A%B8)" title="서담(웹사이트)" data-v-d9583359="">서담(웹사이트)</a> <a class="QuDd1Dh0" href="http://ssodam.com" target="_blank" rel="nofollow noopener" title="http://ssodam.com" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EC%84%9C%EC%9A%B8%EB%8C%80%ED%95%99%EA%B5%90" title="서울대학교" data-v-d9583359="">서울대학교</a> 중앙도서관 <a class="QuDd1Dh0" href="http://library.snu.ac.kr" target="_blank" rel="nofollow noopener" title="http://library.snu.ac.kr" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EC%84%B8%EB%AA%85%EC%BB%B4%ED%93%A8%ED%84%B0%EA%B3%A0%EB%93%B1%ED%95%99%EA%B5%90" title="세명컴퓨터고등학교" data-v-d9583359="">세명컴퓨터고등학교</a> <a class="QuDd1Dh0" href="http://www.smc.hs.kr" target="_blank" rel="nofollow noopener" title="http://www.smc.hs.kr" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359="">러시아어판을 제외한 모든 <a class="sl8O8g9f" href="/w/SCP%20%EC%9E%AC%EB%8B%A8" title="SCP 재단" data-v-d9583359="">SCP 재단</a> 위키.<a class="yDQWz7wG" href="#fn-8" data-v-d9583359=""><span id="rfn-8" data-v-d9583359=""></span>[8]</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EB%B0%B0%EB%AC%B8%EA%B3%A0%EB%93%B1%ED%95%99%EA%B5%90" title="배문고등학교" data-v-d9583359="">배문고등학교</a> <a class="QuDd1Dh0" href="https://baemoon.hs.kr" target="_blank" rel="nofollow noopener" title="https://baemoon.hs.kr" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EC%96%91%EC%98%81%EB%94%94%EC%A7%80%ED%84%B8%EA%B3%A0%EB%93%B1%ED%95%99%EA%B5%90" title="양영디지털고등학교" data-v-d9583359="">양영디지털고등학교</a> <a class="QuDd1Dh0" href="http://www.y-y.hs.kr" target="_blank" rel="nofollow noopener" title="http://www.y-y.hs.kr" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EC%9C%84%ED%82%A4%EB%A6%AC%ED%81%AC%EC%8A%A4" title="위키리크스" data-v-d9583359="">위키리크스한국</a> <a class="QuDd1Dh0" href="http://www.wikileaks-kr.org" target="_blank" rel="nofollow noopener" title="http://www.wikileaks-kr.org" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%EC%9D%B8%EC%8A%A4%ED%83%80%EA%B7%B8%EB%9E%A8" title="인스타그램" data-v-d9583359="">인스타그램</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%ED%8E%80%EC%A6%88%EC%9C%84%ED%82%A4" title="펀즈위키" data-v-d9583359="">펀즈위키</a> <a class="QuDd1Dh0" href="http://funzinnu.com/EVEwiki" target="_blank" rel="nofollow noopener" title="http://funzinnu.com/EVEwiki" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%ED%95%98%EC%9D%B4%ED%84%B0%EC%B9%98" title="하이터치" data-v-d9583359="">하이터치</a> <a class="QuDd1Dh0" href="https://hightch.com/" target="_blank" rel="nofollow noopener" title="https://hightch.com/" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%ED%95%9C%EA%B5%AD%EB%8F%84%EB%A1%9C%EA%B3%B5%EC%82%AC" title="한국도로공사" data-v-d9583359="">한국도로공사</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/%ED%99%A9%EA%B8%88%EA%B3%A0%EB%B8%94%EB%A6%B0" title="황금고블린" data-v-d9583359="">황금고블린</a> <a class="QuDd1Dh0" href="https://golden-goblin.com" target="_blank" rel="nofollow noopener" title="https://golden-goblin.com" data-v-d9583359="">#</a></div></li><li data-v-d9583359=""><div class="agCqF8Vh" data-v-d9583359=""><a class="sl8O8g9f" href="/w/Bootstrap(%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC)" title="Bootstrap(프레임워크)" data-v-d9583359="">Bootstrap(프레임워크)</a> <a class="QuDd1Dh0" href="http://getbootstrap.com/" target="_blank" rel="nofollow noopener" title="http://getbootstrap.com/" data-v-d9583359="">#</a></div></li></ul>

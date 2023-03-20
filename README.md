# 모던 웹을 위한 마이크로 프런트엔드

[《모던 웹을 위한 마이크로 프런트엔드》](https://wikibook.co.kr/micro-frontend/) 저장소입니다.

## 책 소개

<a href="https://wikibook.co.kr/micro-frontend/"><img src="bookcover.jpg" alt="책 표지" height="256px" align="right"></a>

**마이크로 프런트엔드 아키텍처로 복잡성을 해결하고 단일 장애 지점을 제거하자!**

마이크로 프런트엔드는 소프트웨어 개발의 마이크로서비스 개념에서 차용한 프런트엔드 개발을 위한 웹 아키텍처로, 프런트엔드의 복잡성과 단일 장애 지점을 피하기 위해 프런트엔드의 각 모듈을 독립적으로 개발하고 출시한다.

이 책은 따라 하기 쉬운 가이드 형식으로 실습 튜토리얼, 프로젝트 및 자가 평가 질문으로 구성돼 있으며, 마이크로 프런트엔드 솔루션을 구현하는 데 사용할 수 있는 패턴을 안내한다. 마이크로 프런트엔드 일반, 다양한 아키텍처 스타일과 사용 영역, 마이크로 프런트엔드로의 변경에 대비하여 팀을 준비하는 방법, 확장성을 위해 UI 디자인을 조정하는 방법 등을 배울 수 있으며, 마이크로 프런트엔드 아키텍처의 가장 단순한 변형부터 시작하여 정적 접근 방식에서 더 빠른 릴리스 주기로 확장성을 극대화할 수 있는 완전 동적 솔루션까지 다룬다. 마지막 장에서는 마이크로 프런트엔드와 관련된 다양한 사례 연구를 통해 얻은 지식을 강화할 수 있다.

**★ 이 책에서 다루는 내용 ★**

- 올바른 마이크로 프런트엔드 아키텍처를 선택하는 방법
- 컴포지션 UI를 위한 화면 디자인
- 마이크로 프런트엔드 솔루션을 위한 뛰어난 개발자 경험 만들기
- 마이크로 프런트엔드로 향상된 사용자 경험 달성
- 분산된 프런트엔드 관리를 위한 거버넌스 및 경계 검사 도입
- 처음부터 또는 기존 모놀리스를 마이그레이션하여 확장 가능한 모듈식 웹 애플리케이션 구축

### 대상 독자

이 책은 소프트웨어/솔루션 아키텍트 또는 (주로 리드) 개발자, 웹 개발자 및 프론트엔드 엔지니어를 위한 책입니다. HTML과 CSS에 대한 초급 수준의 지식과 함께 자바스크립트 프로그래밍 및 Node.js와 NPM을 포함한 해당 에코시스템에 대한 탄탄한 이해가 전제되어 있습니다.

## 실습 안내

### 저장소 복제

이 리포지터리에는 샘플 코드가 있는 모든 리포지터리들이 포함되어 있습니다. 이러한 리포지터리들은 Git 모듈로 포함되었습니다. 복제할 때 체크아웃하려면 다음과 같이 `--recurse-submodules` 플래그를 추가해야 합니다.

```sh
git clone --recurse-submodules https://github.com/wikibook/micro-frontend.git
```

### 저장소 갱신

서브모듈이 체크아웃되면 이 시점에서 코드가 멈추게 됩니다. 따라서 리포지터리 자체와 마찬가지로 서브모듈도 끌어와야(pull) 합니다.

단일 명령으로 모든 작업을 수행하려면 `--recurse-submodules`와 `git pull`을 함께 사용하면 됩니다.

```sh
git pull --recurse-submodules
```

### 실습

샘플 저장소가 포함된 각 디렉터리에는 필요한 사항과 코드 실행 방법에 대한 지침이 포함된 README 파일이 있습니다(README를 번역해서 책의 부록에 실었습니다).

7장(서버 측 구성)과 11장(사이트리스 UI)의 샘플의 경우 코드가 여러 리포지토리에 분할되어 있습니다. 이는 일반적으로 마이크로프론트엔드의 분산 특성, 특히 주어진 접근 방식의 분산 특성을 설명하기 위해 수행되었습니다.

여기서는 MF 리포지토리를 실행하기 전에 게이트웨이(7장)와 앱 셸(11장)부터 시작하는 것을 권장합니다. 11장의 경우 피드 서버도 실행해야 합니다.

거의 모든 샘플은 HTML 및 JavaScript와 같은 웹 기술만을 사용하여 작성되었습니다. 엣지 사이드 컴포지션 예제(8장)의 경우 nginx 서버를 실행하는 도커 파일이 추가되었습니다.

### 예제 목록

* 5장 - 마이크로프론트엔드 유형
  * [직접 빌드 통합](https://github.com/ArtOfMicrofrontends/05-pipeline)
  * [조회 테이블을 통한 느슨한 커플링](https://github.com/ArtOfMicrofrontends/05-server-discover)
* 6장 - 웹 접근 방식
  * [패턴 예시](https://github.com/ArtOfMicrofrontends/06-web-approach)
* 7장 - 서버 측 구성
  * [MF 오케스트레이션을 위한 게이트웨이](https://github.com/ArtOfMicrofrontends/07-gateway)
  * [상품 페이지를 제공하는 빨간색 MF](https://github.com/ArtOfMicrofrontends/07-red)
  * [구매 기능을 제공하는 파란색 MF](https://github.com/ArtOfMicrofrontends/07-blue)
  * [추천 기능을 제공하는 녹색 MF](https://github.com/ArtOfMicrofrontends/07-green)
* 8장 - 엣지 사이드 구성
  * [패턴 예시](https://github.com/ArtOfMicrofrontends/08-edge-side-composition)
* 9장 - 클라이언트 측 컴포지션
  * [패턴 예시](https://github.com/ArtOfMicrofrontends/09-client-side-composition)
* 10장 - SPA 컴포지션
  * [패턴 예시](https://github.com/ArtOfMicrofrontends/10-spa-composition)
* 11장 - 사이트리스 UI
  * [MF를 오케스트레이션하는 앱 셸](https://github.com/ArtOfMicrofrontends/11-app-shell)
  * [MF를 동적으로 프로비저닝하는 피드 서버](https://github.com/ArtOfMicrofrontends/11-service-feed)
  * [대차 대조표를 가져오는 잔액 MF](https://github.com/ArtOfMicrofrontends/11-frontend-balance)
  * [설정 대화 상자를 제공하는 설정 MF](https://github.com/ArtOfMicrofrontends/11-frontend-settings)
  * [대차 대조표에 대한 확장 기능을 제공하는 세금 MF](https://github.com/ArtOfMicrofrontends/11-frontend-tax)

### 소프트웨어 및 하드웨어

다음 소프트웨어 및 하드웨어 목록을 사용하면 이 책에 있는 모든 코드 파일을 실행할 수 있습니다(1장~16장).

| 필요한 소프트웨어       | 필요한 OS                    |
| -----------------------| ----------------------------|
| Node.js 12             | Windows, Mac OS X 또는 Linux |
| NPM 6                  | Windows, Mac OS X 또는 Linux |
| ECMAScript 2015(6) 이상 | Windows, Mac OS X 또는 Linux |

이 책에 사용된 스크린샷/도표의 컬러 이미지가 포함된 PDF 파일도 제공합니다. [다운로드하려면 여기를 클릭하세요](https://static.packt-cdn.com/downloads/9781800563568_ColorImages.pdf).

## 동영상

코드를 설명한 동영상(영어)이 있습니다.

[YouTube](https://www.youtube.com/playlist?list=PLeLcvrwLe185OWoZT0hfN5zesgVangK5M)

## 오탈자

* [https://wikibook.co.kr/micro-frontend/](https://wikibook.co.kr/micro-frontend/)를 참조

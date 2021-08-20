##### top
# -Study-Nuxt

* [01. ``Nuxt JS`` 프로젝트 생성하기](#01)

* [02. ``Nuxt JS``의 폴더 구조](#02)



<br/><hr/><br/>



* ``Nuxt JS``는 ``Vue`` 프레임워크를 사용한 ``Server Side Rendering Framework`` 입니다.
* ``Nuxt JS`` 프로젝트에는 ``Vuex``, ``Vue-Router``, ``Axios`` 등의 라이브러리들이 미리 구성하여 제공하고 있습니다.

<br/>

``Nuxt JS``를 사용하는 가장 큰 목적은 다음과 같습니다.

* 빠른 페이지 렌더링
* 검색엔진 최적화 (SEO)

<br/>

``Nuxt JS``를 사용할 때는 다음과 같은 사전지식이 필요 합니다.

* ``Node JS``에 대한 지식
* ``Server Side Rendering`` 에 대한 지식
* ``Back End``에 대한 지식

<br/>

``Nuxt JS``를 사용할 때 얻게 되는 장점은 다음과 같습니다.

* 검색엔진 최적화 (SEO)
* 초기 프로젝트 설정이 ``Vue`` 프로젝트에 비해 좀 더 다양하게 제공
* 파일기반(``.vue``) 라우팅 방식으로 동작하므로, 라우터 설정 X



<br/>

[🔺 Top](#top)

<hr/><br/>



##### 01
# 01. ``Nuxt JS`` 프로젝트 생성하기

> 공식홈페이지: [https://ko.nuxtjs.org/docs/2.x/get-started/installation](https://ko.nuxtjs.org/docs/2.x/get-started/installation)

<br/>

``Nuxt JS`` 프로젝트를 생성하기 위한 NPM 명령은 다음과 같습니다. 

(``Nuxt JS``에 대한 설치는 없이, ``NPM 프로젝트 생성 명령``으로 프로젝트를 생성 합니다)

```bash
npm init nuxt-app <프로젝트명>
```

<br/>

위 명령을 실행하면, 다음과 같은 프로젝트 생성 설정을 할 수 있습니다.

각 설정 단계에서 필요한 것들을 선택할 수 있는데, 설정 중 ``Rendering Mode``에는 다음과 같은 설정을 할 수 있습니다.

* ``Universal (SSR / SSG)``
* ``Single Page App``

``Universal (SSR / SSG)``의 경우, ``Server Side Rendering`` 또는 ``Static Site Generator`` 프로젝트가 생성 됩니다.

그리고, ``Single Page App``의 경우, 기존의 ``Vue``프로젝트 처럼 ``Client Side Rendering`` 프로젝트가 생성 됩니다.

그러므로, 현재는 ``Server Side Rendering`` 프로젝트를 위한 ``Nuxt JS``를 사용하기 위해, ``Universal`` 모드를 선택 합니다.

<img src="./readmeAssets/01-nuxtjs-프로젝트-생성하기-01.png" width="700px" alt="이미지: Nuxt JS 프로젝트 생성 01"><br/>

<br/>

``Universal`` 모드 프로젝트를 선택하게 되면, ``배포 방식``을 설정하게 되는데, 현재 우리가 만들 프로젝트는 ``Server Side Rendering`` 이므로, ``Server (Node.js hosting)`` 을 선택 합니다.

<img src="./readmeAssets/01-nuxtjs-프로젝트-생성하기-02.png" width="700px" alt="이미지: Nuxt JS 프로젝트 생성 02"><br/>

<br/>

다음 설정으로는 개발툴에 대한 설정을 할 수 있습니다. (``Development Tools``)

``VSCode``를 사용한다면, ``jsconfig.json``으로 설정하면 됩니다.

<img src="./readmeAssets/01-nuxtjs-프로젝트-생성하기-03.png" width="700px" alt="이미지: Nuxt JS 프로젝트 생성 03"><br/>

<br/>

``Nuxt JS`` 프로젝트 생성이 완료되면, 다음과 같은 안내를 받을 수 있습니다.

<img src="./readmeAssets/01-nuxtjs-프로젝트-생성하기-04.png" width="700px" alt="이미지: Nuxt JS 프로젝트 생성 04"><br/>

<br/>

``Nuxt JS``의 개발서버 실행은 ``dev`` 명령으로 설정되어 있습니다.

```bash
$ npm run dev
```

실행하게 되면 ``http://localhost:3000/`` 경로로 실행할 수 있습니다.

<img src="./readmeAssets/01-nuxtjs-프로젝트-생성하기-05.png" width="700px" alt="이미지: Nuxt JS 프로젝트 생성 05"><br/>

<br/>

아래 이미지는 ``Nuxt JS`` 프로젝트를 생성한 직후의 실행 화면 입니다.

<img src="./readmeAssets/01-nuxtjs-프로젝트-생성하기-06.png" width="700px" alt="이미지: Nuxt JS 프로젝트 생성 06"><br/>

<br/>

``Nuxt JS`` 프로젝트를 실행중에 소스코드가 변경되면, 해당 사항은 자동으로 반영되므로, 서버를 재실행할 필요는 없습니다.



<br/>

[🔺 Top](#top)

<hr/><br/>



##### 02
# 02. ``Nuxt JS``의 폴더 구조

<img src="./readmeAssets/02-nuxtjs-폴더구조-01.png" width="400px" alt="이미지: 폴더구조"><br/>

* ``.nuxt``: ``Nuxt JS`` 프로젝트 개발서버 실행 시, ``빌드결과물`` 폴더 입니다. (``.gitignore`` 설정상태)
* ``components``: ``Vue 컴포넌트`` 폴더
* ``pages``: ``Nuxt JS`` 프로젝트의 페이지용 ``Vue 컴포넌트`` 폴더
* ``static``: 정적 리소스 폴더
* ``store``: ``Vuex`` 폴더
* ``nuxt.config.js``: ``Nuxt JS`` 프로젝트 설정파일



<br/>

[🔺 Top](#top)

<hr/><br/>



##### 03
# 03. 
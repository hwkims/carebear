## CareBear - AI 말벗 로봇 🐻👵👴

[https://hwkims.github.io/carebear/](https://hwkims.github.io/carebear/)

CareBear는 독거 노인 👴👵 분들을 위한 치매 예방 🧠 및 정서적 안정 💖을 돕는 음성 기반 AI 대화 로봇 🤖입니다. ChatGPT API를 활용하여 맞춤형 대화를 제공하고, 사용자의 감정을 케어하는 데 중점을 둡니다. 이 프로젝트는 위시켓의 [ChatGPT 기반 치매 예방 및 감정 케어 목적의 음성 기반 AI 대화 로봇 개발](https://www.wishket.com/project/142168/) 프로젝트의 MVP(최소 기능 제품) 개발을 위해 만들어졌습니다.

### ✨ 주요 기능 ✨

*   **👵👴 맞춤형 대화:** ChatGPT API를 활용하여 독거 노인에게 적합한 맞춤형 대화를 생성합니다. 1,000개 이상의 대화 예제를 기반으로 파인 튜닝 및 프롬프팅을 할 수 있습니다(현재는 미적용).
*   **💖 감정 케어:** 사용자의 감정(기쁨 😄, 슬픔 😭, 분노 😡 등)을 파악하고, 대화에 반영하여 정서적 지원을 제공합니다. (간단한 로직 사용, 추후 감정 인식 알고리즘 연동 예정).
*   **🎤 음성 인터페이스:** 노인 분들이 쉽게 사용할 수 있도록 음성 기반 UI/UX를 설계했습니다. STT(Speech-to-Text) 및 TTS(Text-to-Speech) 변환 기능을 모두 제공합니다.
*   **📊 데이터 분석:** (추후 구현 예정) 사용자 대화 데이터를 수집하고 분석하여 서비스 개선에 활용합니다. 관리자 페이지에서 데이터를 확인할 수 있습니다.
*   **☁️ 클라우드 기반:** (추후 구현 예정) 1년 동안 안정적인 서비스 운영을 위해 클라우드 서버를 구축할 예정입니다 (약 100명 사용자 기준).

### 🚀 시작하기 🚀

1.  **리포지토리 복제:**

    ```bash
    git clone https://github.com/hwkims/carebear.git
    cd carebear
    ```

2.  **OpenAI API 키 얻기:**
    *   [OpenAI 웹사이트](https://platform.openai.com/)에 가입합니다.
    *   계정 대시보드에서 API 키를 생성합니다.

3.  **API 키 구성:**
    *   텍스트 편집기에서 `index.html` 파일을 엽니다.
    *   다음 줄을 찾습니다:

        ```javascript
        let apiKey = localStorage.getItem('openaiApiKey') || '';
        ```
        * 이 코드 위에 아래의 코드를 삽입합니다.
        ```javascript
         // OpenAI API Key (Replace with your actual API key)
        const apiKey = 'YOUR_OPENAI_API_KEY';
        ```
         `YOUR_OPENAI_API_KEY` 이 부분을 실제 API키로 변경합니다.

    ⚠️ **중요 보안 참고:** 프로덕션 환경에서는 API 키를 안전하게 관리하고 OpenAI API에 대한 요청을 처리하기 위해 백엔드 서버를 사용하는 것이 좋습니다. 클라이언트 측 코드에 직접 API 키를 저장하는 것은 보안상 위험합니다.

4.  **브라우저에서 열기:**
    *   웹 브라우저에서 `index.html` 파일을 엽니다.

### ☁️ 배포 ☁️

CareBear는 GitHub Pages와 같은 플랫폼에 쉽게 배포할 수 있습니다.

1.  **코드를 hwkims/carebear 리포지토리에 푸시:**

    *   이미 리포지토리를 클론한 상태이므로, 수정된 `index.html` 파일을 커밋하고 푸시합니다.

2.  **GitHub Pages 활성화:**
    *   [hwkims/carebear 리포지토리](https://github.com/hwkims/carebear)의 설정으로 이동합니다.
    *   "Pages" 섹션에서 "Source"를 "main" (또는 사용하는 분기)으로 설정하고 "Save"를 클릭합니다.

3.  **사이트 액세스:**
    *   GitHub Pages가 활성화되면 몇 분 안에 [https://hwkims.github.io/carebear/](https://hwkims.github.io/carebear/) 에서 CareBear에 액세스할 수 있습니다.

### 🛠️ 기술 스택 🛠️

*   **AI:** ChatGPT API (GPT-3.5-turbo)
*   **프론트엔드:** HTML, CSS, JavaScript
*   **음성 인식/합성:** Web Speech API
*   **서버:** (현재는 없음, 백엔드 서버 구축 시 추가 예정)

### 🤝 참여 방법 🤝

CareBear 프로젝트에 기여하고 싶다면 언제든지 풀 리퀘스트를 제출해주세요! 🐛 발견, 💡 아이디어, 🎨 디자인 개선 등 어떤 기여든 환영합니다.

### 📜 라이선스 📜

이 프로젝트는 MIT 라이선스에 따라 사용이 허가됩니다. 자세한 내용은 `LICENSE` 파일을 참조하십시오.

---

**hwkims** 제작

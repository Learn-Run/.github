

![image](https://github.com/user-attachments/assets/a719da44-7838-4b06-a10e-fc124dce04d5)





# Front

## 📚 프로젝트 소개 및  개요
---
프로젝트 기간 : 2025.05.06 ~ 2025.07.15
배포 URL : [pick-learn](https://pickandlearn.shop/)


[프로젝트 설명]
- AI 가 빠르게 발전하며 정보 접근이 쉬워진 시대, 질문하고, 답하고 서로의 지식과 경험을 나눌 수 있는 AI 가 아닌 사람 중심의 실시간 지식 공유 플랫폼입니다 

<details>
<summary>목차</summary>
<div markdown="1">

1. [팀 소개](#teamintro)
2. [기술 및 개발 환경](#stack)
3. [개발 기간 및 작업 문화](#task)
4. [주요 기능](#mainfeat)
5. [역할분담](#role)
6. [UI](#ui)
7. [기능](#pageinfo)
8. [느낀점](#impression)
</div>
</details>
<br/>


## <span id="teamintro">1. 팀 소개</span>
### 🚀 Learn-Run 팀을 소개합니다!
안녕하세요, 저희는 2명의 Front-end, 2명의 Back-end 개발자로 구성된 **Learn-Run**팀입니다. </br>
배우면 바로 실천하고 달리는 팀 이라는 의미로, 새로운 기술이나 도전을 머뭇거리지 않고 빠르게 흡수하고 적용하는 실행력 중심의 팀
</br>

&nbsp;

## 🛠 기술 스택

| 카테고리                  | 스택                                                                                                                                                                                                          | 사용 목표                                         |
| :------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :------------------------------------------------ |
| **Programming Languages** | ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=TypeScript&logoColor=white)                                                                                               | 코드 안정성 및 유지보수성 향상을 위함             |
| **Frameworks**            | ![React](https://img.shields.io/badge/React-06B6D4?style=flat-square&logo=React&logoColor=white) ![Next.js](https://img.shields.io/badge/next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)     | 컴포넌트 기반 SSR 및 SSG, SEO 최적화              |
| **CSS Framework**         | ![Tailwind CSS](https://img.shields.io/badge/tailwindcss-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)                                                                                           | 유틸리티 클래스 CSS 프레임워크를 통한 개발 최적화 |
| **UI Library**            | ![Shadcn/ui](https://img.shields.io/badge/shadcn/ui-000000?style=flat-square&logo=shadcn/ui&logoColor=white)                                                                                                  | 재사용 가능한 고품질 컴포넌트 라이브러리          |
| **Build System**          | ![Turborepo](https://img.shields.io/badge/Turborepo-000000?style=flat-square&logo=turborepo&logoColor=white)                                                                                                  | 고성능 빌드 시스템과 모노레포 관리                |
| **Package Manager**       | ![pnpm](https://img.shields.io/badge/pnpm-000000?style=flat-square&logo=pnpm&logoColor=white)                                                                                                                 | 빠르고 효율적인 패키지 매니저                     |
| **Development Tools**     | ![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=flat-square&logo=eslint&logoColor=white) ![Prettier](https://img.shields.io/badge/Prettier-F7B93E?style=flat-square&logo=prettier&logoColor=white) | 코드 품질 및 일관성 유지                          |

&nbsp;

## 📁 프로젝트 구조

[FRONT]

```bash
📦learn-run-front
 ┣ 📂apps
 ┃ ┣ 📂pick-learn               # 학습 플랫폼 애플리케이션
 ┃ ┃ ┣ 📂src
 ┃ ┃ ┃ ┣ 📂app
 ┃ ┃ ┃ ┃ ┣ 📂(home)            # 홈 레이아웃
 ┃ ┃ ┃ ┃ ┃ ┣ 📂sign-up         # 회원가입
 ┃ ┃ ┃ ┃ ┃ ┣ 📂sign-in         # 로그인
 ┃ ┃ ┃ ┃ ┃ ┣ 📂post            # 게시글 관리
 ┃ ┃ ┃ ┃ ┃ ┣ 📂profile         # 프로필 관리
 ┃ ┃ ┃ ┃ ┃ ┣ 📂payment         # 결제 시스템
 ┃ ┃ ┃ ┃ ┃ ┣ 📂search          # 검색 기능
 ┃ ┃ ┃ ┃ ┃ ┗ 📂@modal          # 모달 컴포넌트
 ┃ ┃ ┃ ┗ 📂components           # 공통 컴포넌트
 ┃ ┃ ┗ 📂public                 # 정적 파일
 ┃ ┗ 📂chat-service             # 채팅 서비스 애플리케이션
 ┃   ┣ 📂src
 ┃   ┃ ┣ 📂app
 ┃   ┃ ┃ ┣ 📂(home)            # 홈 레이아웃
 ┃   ┃ ┃ ┃ ┣ 📂home            # 홈 페이지
 ┃   ┃ ┃ ┃ ┣ 📂messages        # 메시지 관리
 ┃   ┃ ┃ ┃ ┣ 📂profile         # 프로필 관리
 ┃   ┃ ┃ ┃ ┗ 📂@modal          # 모달 컴포넌트
 ┃   ┃ ┃ ┗ 📂api               # API 라우트
 ┃   ┃ ┗ 📂features            # 기능별 컴포넌트
 ┃   ┗ 📂public                 # 정적 파일
 ┣ 📂packages
 ┃ ┣ 📂ui                        # 공유 UI 컴포넌트 (Shadcn/ui)
 ┃ ┃ ┣ 📂src
 ┃ ┃ ┃ ┣ 📂components           # UI 컴포넌트
 ┃ ┃ ┃ ┃ ┣ 📂base              # 기본 컴포넌트
 ┃ ┃ ┃ ┃ ┗ 📂wrapper           # 래퍼 컴포넌트
 ┃ ┃ ┃ ┣ 📂styles              # 스타일 정의
 ┃ ┃ ┃ ┣ 📂lib                 # 유틸리티
 ┃ ┃ ┃ ┗ 📂assets              # 아이콘 및 이미지
 ┃ ┃ ┗ 📂components.json        # Shadcn/ui 설정
 ┃ ┣ 📂eslint-config            # ESLint 설정
 ┃ ┗ 📂typescript-config        # TypeScript 설정
 ┣ 📂.github                     # GitHub Actions 및 템플릿
 ┣ 📂.husky                      # Git hooks 설정
 ┗ 📂turbo.json                  # Turborepo 설정
```

&nbsp;

## 역할 분담

### 👨‍💻 Front-end

#### Learn-Run Frontend Team

| 기능                | 구현 목록                                                                 | 설명                                                                                                                             |
| :------------------ | :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------- |
| **pick-learn 앱**   | 학습 플랫폼<br>회원가입/로그인<br>게시글 관리<br>결제 시스템<br>검색 기능 | - 학습 플랫폼으로서의 핵심 기능들을 구현했습니다.<br>- Next.js App Router를 활용한 모던한 라우팅 구조를 구축했습니다.            |
| **chat-service 앱** | 실시간 채팅<br>메시지 관리<br>프로필 관리<br>API 라우트                   | - 실시간 채팅 기능을 위한 별도 애플리케이션을 구축했습니다.<br>- NextAuth를 활용한 인증 시스템을 구현했습니다.                   |
| **공유 UI 시스템**  | Shadcn/ui 컴포넌트<br>Tailwind CSS v4<br>기본/래퍼 컴포넌트               | - 두 앱에서 공유하는 UI 컴포넌트 라이브러리를 구축했습니다.<br>- 재사용 가능한 컴포넌트 구조로 개발 효율성을 높였습니다.         |
| **모노레포 관리**   | Turborepo 설정<br>Workspace 관리<br>빌드 최적화                           | - Turborepo를 활용한 고성능 모노레포 환경을 구축했습니다.<br>- 여러 앱과 패키지를 효율적으로 관리할 수 있는 구조를 설계했습니다. |

&nbsp;

## ⚙️ 프로젝트 실행 방법

프론트엔드 프로젝트를 실행하기 전 아래 항목들을 확인해주세요.

- Node.js 18.0.0 이상이 설치되어 있어야 합니다.
- pnpm 8.0.0 이상이 설치되어 있어야 합니다.

### 환경변수(.env)

```bash
# Next.js 설정
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your-secret-key

# API 설정
NEXT_PUBLIC_API_URL=http://localhost:8000

# 기타 설정
NODE_ENV=development
```

## 📦 Getting Started

1. **프로젝트 클론**

```bash
git clone https://github.com/Learn-Run/front.git
```

2. **프로젝트 디렉토리로 이동**

```bash
cd front
```

3. **의존성 설치**

```bash
pnpm install
```

4. **개발 서버 실행**

```bash
turbo dev --filter nextjs
```

5. **앱 확인**

- 앱이 정상적으로 실행되면 로컬 주소를 통해 앱을 확인할 수 있습니다.
- http://localhost:3000

&nbsp;

## 🎯 주요 기능

### 🏗️ 모노레포 아키텍처

- **Turborepo**: 빌드 캐싱과 병렬 실행으로 빠른 개발
- **Workspace**: 패키지 간 효율적인 의존성 관리
- **Shared Packages**: UI 컴포넌트와 설정의 재사용
- **Incremental Builds**: 변경된 부분만 빌드하여 개발 속도 향상
- **Remote Caching**: 팀원 간 빌드 결과 공유

### 🎨 현대적인 UI 시스템

- **Shadcn/ui**: 접근성과 커스터마이징이 뛰어난 컴포넌트
- **Tailwind CSS v4**: 최신 기능과 향상된 성능
- **Dark Mode**: 자동 다크모드 지원 및 테마 전환
- **Responsive Design**: 모든 디바이스에서 완벽한 경험
- **Component Library**: 재사용 가능한 UI 컴포넌트 모음
- **Custom Themes**: 브랜드에 맞는 테마 커스터마이징

### ⚡ 개발자 경험

- **Hot Reload**: 실시간 코드 변경 반영
- **Type Safety**: TypeScript를 통한 런타임 에러 방지
- **Code Quality**: ESLint와 Prettier를 통한 일관된 코드 스타일
- **Git Hooks**: 커밋 전 자동 코드 검사
- **VS Code Integration**: 자동 완성 및 린팅 지원

### 🚀 프로덕션 준비 기능

- **Optimized Builds**: 자동 코드 분할 및 최적화
- **SEO Ready**: 메타데이터 및 구조화된 데이터 지원
- **Performance Monitoring**: Core Web Vitals 최적화
- **Accessibility**: WCAG 2.1 AA 준수 컴포넌트
- **Internationalization**: 다국어 지원 준비

### 🔧 개발 도구

- **Component Generator**: Shadcn/ui CLI를 통한 컴포넌트 자동 생성
- **Storybook Integration**: 컴포넌트 문서화 및 테스트
- **Testing Setup**: Jest, React Testing Library 설정
- **Docker Support**: 컨테이너화 및 배포 준비
- **CI/CD Ready**: GitHub Actions 워크플로우 포함

### 📱 반응형 및 접근성

- **Mobile First**: 모바일 우선 디자인
- **Touch Friendly**: 터치 인터페이스 최적화
- **Screen Reader**: 스크린 리더 지원
- **Keyboard Navigation**: 키보드 네비게이션 지원
- **High Contrast**: 고대비 모드 지원

&nbsp;

## 🛠 개발 가이드

### 새로운 컴포넌트 추가

```bash
cd packages/ui
pnpm dlx shadcn@latest add [component-name]
```

### 새로운 앱 추가

```bash
cd apps
npx create-next-app@latest my-new-app --typescript --tailwind --eslint
```

### 빌드 및 배포

```bash
# 개발 빌드
turbo build --filter nextjs

# 프로덕션 빌드
turbo build --filter=nextjs --filter=ui

# 린트 검사
turbo lint

# 타입 검사
turbo type-check
```

&nbsp;

## 🔧 설정 파일

### Tailwind CSS v4 설정

가장 중요한 설정은 `apps/nextjs/src/app/globals.css` 파일입니다:

```css
@import "tailwindcss";
@import "@repo/ui/styles/default.css";

@source '../../node_modules/@repo/ui';
```

### Shadcn/ui 설정

`packages/ui/components.json`에서 테마와 스타일을 커스터마이징할 수 있습니다.

&nbsp;

## 🤝 기여하기

1. 이 저장소를 Fork합니다
2. 새로운 기능 브랜치를 생성합니다 (`git checkout -b feature/amazing-feature`)
3. 변경사항을 커밋합니다 (`git commit -m 'Add some amazing feature'`)
4. 브랜치에 Push합니다 (`git push origin feature/amazing-feature`)
5. Pull Request를 생성합니다

&nbsp;

## 📝 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

&nbsp;

## 🙏 감사의 말

이 보일러플레이트는 다음 오픈소스 프로젝트들의 도움을 받았습니다:

- [Turborepo](https://turbo.build/repo) - 고성능 빌드 시스템
- [Shadcn/ui](https://ui.shadcn.com/) - 아름다운 UI 컴포넌트
- [Tailwind CSS](https://tailwindcss.com/) - 유틸리티 퍼스트 CSS 프레임워크
- [Next.js](https://nextjs.org/) - React 풀스택 프레임워크

---

**Learn-Run Frontend** - 현대적인 웹 개발의 새로운 시작점 🚀

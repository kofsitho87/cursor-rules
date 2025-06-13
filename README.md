# Cursor Rules 모음집

이 프로젝트는 다양한 개발 환경과 기술 스택을 위한 Cursor Rules 가이드라인을 제공합니다. 각 환경별로 최적화된 코딩 스타일, 프로젝트 구조, 라이브러리 활용 규칙 및 모범 사례를 담고 있어 개발 팀의 생산성과 코드 품질을 향상시킬 수 있습니다.

## 프로젝트 구조

*   `frontend/`: Next.js 15 + TypeScript 프론트엔드 개발용 Cursor Rules
*   `backend/`: 백엔드 개발용 Cursor Rules 가이드라인
*   `python/`: Python 개발용 Cursor Rules (Langchain, Langgraph 등 AI 관련 포함)
*   `README.md`: 프로젝트 개요 및 사용법

## Frontend

프론트엔드는 **Next.js 15.3**과 **TypeScript**를 기반으로 구성되어 있으며, **App Router**를 사용합니다. 주요 기술 스택은 다음과 같습니다.

*   **UI**: `Tailwind CSS`, `shadcn/ui`, `Lucide React`
*   **상태 관리**: `React Query` (서버), `nuqs` (URL)
*   **폼**: `React Hook Form` + `Zod`
*   **테이블**: `TanStack Table`
*   **퍼널 플로우**: `@use-funnel/browser`
*   **React 유틸리티**: `react-simplikit` (경량 React 전용 라이브러리)

`react-simplikit`은 React의 설계 원칙을 존중하면서 개발 경험을 개선하는 경량 라이브러리입니다. SSR 환경에서 안전하고, 제로 의존성으로 번들 사이즈를 최적화하며, 토글 상태 관리, 디바운스 처리, 외부 클릭 감지, 교차 관찰 등의 유용한 훅과 컴포넌트를 제공합니다.

### 개발 가이드라인

*   **[Next.js (TypeScript)](frontend/nextjs-typescript.mdc)** - Next.js 15.3 + TypeScript 프로젝트의 코딩 스타일, 프로젝트 구조, 라이브러리 활용 규칙 및 모범 사례 (react-simplikit 활용법 포함)

# Cursor Rules 관리 프로젝트

이 프로젝트는 Cursor-related rules를 효율적으로 관리하고 적용하기 위한 시스템입니다. 웹 애플리케이션을 통해 규칙을 손쉽게 생성, 수정, 조회 및 삭제할 수 있는 인터페이스를 제공하며, Python 기반의 백엔드를 통해 복잡한 규칙 처리 및 분석을 수행합니다.

## 주요 기능

*   **웹 기반 규칙 관리**: 사용자는 직관적인 웹 UI를 통해 규칙을 관리할 수 있습니다.
*   **강력한 백엔드**: Python과 Langchain/Langgraph를 활용하여 유연하고 확장 가능한 규칙 엔진을 제공합니다.
*   **다양한 규칙 지원**: 다양한 종류의 Cursor rules를 지원하며, 필요에 따라 새로운 규칙 유형을 쉽게 추가할 수 있습니다.

## 프로젝트 구조

*   `frontend/`: React 또는 다른 최신 프레임워크 기반의 웹 애플리케이션
*   `backend/`: 규칙 처리 로직 및 API를 담당하는 서버
*   `python/`: Langchain 및 Langgraph를 활용한 핵심 규칙 엔진 및 AI 관련 모듈
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

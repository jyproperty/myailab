# 디자인 시스템

## 컬러 팔레트
- Primary: #1976d2 (MUI 기본 블루)
- Secondary: #dc004e (MUI 기본 핑크)
- Background: #ffffff
- Surface: #f5f5f5
- Error: #f44336

## 타이포그래피
- Font Family: Roboto (Google Fonts)
- H1: 2.125rem / 500
- H2: 1.5rem / 500
- H3: 1.25rem / 500
- Body1: 1rem / 400
- Body2: 0.875rem / 400

## 간격 (Spacing)
- 기본 단위: 8px
- xs: 4px (0.5)
- sm: 8px (1)
- md: 16px (2)
- lg: 24px (3)
- xl: 32px (4)

## 컴포넌트 원칙
- MUI 컴포넌트 우선 사용
- 커스텀 스타일은 sx prop 또는 styled() 사용
- 반응형: xs → sm → md → lg → xl 순서로 설계

## 그리드 시스템
- 12컬럼 기반
- Container maxWidth: 'lg' (1200px)
- 기본 padding: 24px (양쪽)

# 새 프로젝트 생성 가이드

## _template_settings 기반 빠른 시작

### 1단계: 템플릿 복사
```bash
# lecture1 디렉토리에서 실행
cp -r _template_settings [새프로젝트명]
cd [새프로젝트명]
```

### 2단계: 프로젝트 이름 변경
`package.json`의 `name` 필드를 프로젝트명으로 변경:
```json
{
  "name": "새프로젝트명",
  ...
}
```

### 3단계: 개발 서버 시작
```bash
npm run dev
```

## 새로 설치가 필요한 경우

### Vite + React 프로젝트 생성
```bash
npm create vite@latest [프로젝트명] -- --template react
cd [프로젝트명]
npm install
```

### MUI 패키지 설치
```bash
npm install react-router-dom @mui/material @emotion/react @emotion/styled @mui/icons-material @fontsource/roboto
```

### theme.js 생성
`src/theme.js`를 생성하고 MUI 테마를 설정합니다.

### main.jsx 수정
ThemeProvider와 CssBaseline을 적용합니다.

## 포함된 패키지 목록
- react + react-dom: UI 라이브러리
- react-router-dom: 클라이언트 라우팅
- @mui/material: MUI 컴포넌트
- @emotion/react + @emotion/styled: MUI 스타일링 엔진
- @mui/icons-material: MUI 아이콘
- @fontsource/roboto: Roboto 폰트

# 코드 컨벤션

## 파일 명명 규칙
- 컴포넌트: PascalCase (예: UserProfile.jsx)
- 훅: camelCase + use 접두사 (예: useUserData.js)
- 유틸리티: camelCase (예: formatDate.js)
- 상수: UPPER_SNAKE_CASE (예: API_BASE_URL)

## 컴포넌트 구조
```jsx
// 1. imports
import React, { useState } from 'react'
import { Box, Typography } from '@mui/material'

// 2. 컴포넌트 정의
function ComponentName({ prop1, prop2 }) {
  // 3. 상태 선언
  const [state, setState] = useState(null)

  // 4. 이벤트 핸들러
  const handleClick = () => {}

  // 5. JSX 반환
  return (
    <Box>
      <Typography>{prop1}</Typography>
    </Box>
  )
}

export default ComponentName
```

## 폴더 구조
```
src/
├── components/     # 재사용 컴포넌트
├── pages/          # 페이지 컴포넌트
├── hooks/          # 커스텀 훅
├── utils/          # 유틸리티 함수
├── constants/      # 상수
├── theme.js        # MUI 테마
└── main.jsx        # 엔트리포인트
```

## 스타일링 원칙
- sx prop: 단순한 인라인 스타일
- styled(): 재사용 필요한 복잡한 스타일
- CSS 모듈: 전역 스타일 피하기

## import 순서
1. React/라이브러리
2. MUI 컴포넌트
3. 내부 컴포넌트
4. 훅/유틸
5. 스타일/이미지

# ROSE AGE

40대 탄력 케어 랜딩 페이지. 정적 HTML이며 GitHub + Vercel 배포를 기준으로 구성했습니다.

## 로컬 확인

```bash
npx --yes serve .
```

브라우저에서 `http://localhost:3000` 을 엽니다.

## 배포 전 설정

`index.html` 하단 `CONFIG`에서 Google Form 주소를 넣으면 CTA 버튼이 설문으로 연결됩니다.

```js
const CONFIG = {
  FORM_URL: 'https://forms.gle/xxxxxxxx',
  PASS_UTM: true,
};
```

비워 두면 버튼 클릭 시 “설문 링크가 아직 연결되지 않았어요” 안내가 나옵니다.

## Vercel

1. [Vercel](https://vercel.com)에 GitHub 계정으로 로그인합니다.
2. **Add New… → Project**에서 이 저장소를 Import합니다.
3. Framework Preset은 **Other**, Root Directory는 `.` 그대로 둡니다.
4. Deploy를 누르면 `index.html`이 사이트 루트로 제공됩니다.

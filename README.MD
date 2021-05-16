# 로그인 컨트롤 (Login Control )

특정 사용자에 대한 로그인 토큰을 모두 삭제해주는 Home Assistant 커스텀 컴포넌트입니다.

## 사용법:
1. HomeAssistant의 configuration.yaml 파일에 `login_control:` 을 추가하여 커스텀 컴포넌트를 활성화 합니다. (재부팅 필요)
2. 로그인 토큰을 초기화하기 원하는 사용자 ID를 식별합니다. (구성하기 -> 사용자 -> 사용자 클릭 하여 나타나는 팝업 윈도우 창에서 'c4571fb4aee04fad83d6b85b0649a4b9' 형태의 ID값을 확인 가능합니다.)
3. `clear_refresh_tokens` 서비스 호출 시에 `user_id` 파라메타에 위의 사용자 ID값을 전달하여 본 컴포넌트의 사용이 가능합니다.

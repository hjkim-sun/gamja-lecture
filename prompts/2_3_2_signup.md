curriculum.md 파일을 참고하여 두 번째 단계인 회원가입·로그인을 개발한다. 
개발 시 orca orchestration을 사용하도록 하며 아래 순서로 진행한다.

설계문서 생성 -> 검토(사람) -> 프론트 엔드 개발 
                      |-> 백엔드 개발 

각 단계에 띄울 워커 에이전트는 아래와 같다.
설계문서 생성:
 - agent: codex
 - model: gpt-6-astra
 - effort: medium

프론트엔드 개발:
 - agent: claude
 - model: opus
 - effort: high

백엔드 개발:
 - agent: codex
 - model: gpt-5.6-terra
 - effort: high

프론트엔드와 백엔드 개발은 동시에 수행한다. 
워커를 띄우면 워커의 터미널 명은 design/front/backend 등 역할에 맞는 이름으로 지정한다.  

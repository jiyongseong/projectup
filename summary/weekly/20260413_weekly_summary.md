# Azure 주간 업데이트 요약 - 2026년 04월 13일

## 🧬 Microsoft Foundry

Microsoft Foundry는 대규모 AI 및 데이터 파이프라인 관리, 고급 모델 배포, 개발 생산성 향상에 중점을 두고 다양한 혁신을 보여주고 있습니다. 최근 GigaTIME 등 멀티모달 AI 모델의 헬스케어 적용, Cohere Transcribe와 Nanbeige 등 오픈소스 모델의 신속한 도입, Grok 4.2·4.20과 같은 제너러티브 AI 지원 확대가 두드러집니다. Foundry Labs에서는 MAI-Voice, VibeVoice ASR, harrier-oss 등 멀티모달/음성/비전 모델을 실험할 수 있는 환경을 제공합니다. 수백만 디바이스에 사설 온디바이스 AI 추론을 지원하는 Foundry Local이 정식 지원으로 출시되며, 통합 모델 카탈로그·엔드포인트 기반의 배포와 비용 관리 기능이 추가되어 엔터프라이즈급 AI 관리 체계를 완성했습니다. 오픈 소스 생태계 확장, 서드파티 가드레일 통합을 통해 안전성 관리도 한층 강화되었습니다.

### [Foundry Local 정식 지원](https://devblogs.microsoft.com/foundry/foundry-local-ga/)
수백만 디바이스에 빠르고 프라이빗한 온프레미스 AI 추론을 즉시 배포할 수 있으며, 토큰당 과금 없이 고성능 추론 환경을 제공합니다.

### [Foundry에 도입된 Cohere Transcribe, Nanbeige 4.1-3B, Octen Embedding](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/now-in-foundry-cohere-transcribe-nanbeige-4-1-3b-and-octen/ba-p/4508183)
음성인식, 추론, 시맨틱 임베딩 등 오픈소스 AI 모델 3종이 배포되어 다국어와 도메인 특화 활용이 보다 강화되었습니다.

### [2026년 3월 Foundry 주요 업데이트](https://devblogs.microsoft.com/foundry/whats-new-in-microsoft-foundry-mar-2026/)
GPT-5.4, Phi-4 Vision, Fireworks AI, Palo Alto 가드레일 등 신규 모델 및 에이전트, 다양한 개발 SDK 정식 지원으로 AI 서비스 범위가 크게 확장되었습니다.


## 🪐 Microsoft Fabric

Microsoft Fabric은 전사적 데이터·AI 분석 플랫폼으로서 실시간 데이터 분석, CDC 통합, 쿼리 성능, 모델링 유연성 등에서 혁신을 이어가고 있습니다. ALTER TABLE 작업의 트랜잭션 처리(정식 지원)로 데이터 무결성을 보장하면서, 실시간 분석 엔진(Eventhouse 엔드포인트), Throttling 모니터, RTD 대시보드 실시간 갱신 등 운영 효율이 크게 개선되었습니다. DAX 사용자 정의 함수, ANY_VALUE 함수가 추가되어 복잡한 비즈니스 로직을 모델링에 유연하게 적용할 수 있고, CDC 기능의 정식 지원으로 자동화 파이프라인 구축이 쉬워졌습니다. 풍부한 파일 포맷 지원, 실시간 스트림·배치 통합, 다양한 커넥터 및 멀티 클라우드 지원 등도 Fabric의 경쟁력을 높였습니다.

### [ALTER TABLE 트랜잭션 지원(정식 지원)](https://www.fabric-gps.com/release/efc9cb1a-4597-f011-b4cc-6045bd00f9db)
스키마 변경이 트랜잭션 단위로 적용되어 자동화 및 CI/CD 파이프라인에서 데이터 무결성과 롤백 보장이 강화되었습니다.

### [Eventhouse 엔드포인트(정식 지원 예정)](https://www.fabric-gps.com/release/e2e8767a-5df1-f011-8406-6045bd026004)
실시간 및 스트리밍 쿼리가 통합 지원되어 반응성이 대폭 개선되고, KQL 기반 실시간 쿼리와 배치 분석의 통합을 실현합니다.

### [Copy Job - Change Data Capture 기능 정식 지원](https://www.fabric-gps.com/release/c4e7283e-6821-f011-998a-0022480939f0)
Copy Job에 CDC(변경 데이터 캡처) 지원이 추가되어, 실시간 데이터 동기화와 데이터 통합 자동화가 훨씬 수월하게 구현됩니다.


## 🧑‍💻 인프라 & 컨테이너 & 데이터베이스

Azure 인프라 영역에서는 GPU VM 지원 확장, 컨테이너 네트워크 관리, 데이터베이스 연결 효율화 등이 핵심입니다. OpenShift는 최신 H100·H200 GPU를 공식 지원해 대규모 AI/머신러닝, HPC 환경에 최적화되었습니다. AKS는 Pod CIDR 영역 확장과 HTTP 프록시 관리 기능으로 네트워크 정책 유연성이 크게 향상됐으며, 쿠버네티스의 운영/확장성이 강화됐습니다. Azure Database for PostgreSQL은 내장 PgBouncer 기능을 정식 지원해 대형 트랜잭션 환경에서 커넥션 풀링과 안정성이 높아졌습니다.

### [Azure Red Hat OpenShift의 NVIDIA H100/H200 GPU 지원](https://azure.microsoft.com/updates?id=559547)
최신 AI 및 고성능 컴퓨팅 워크로드에 특화된 GPU 기반 VM 지원이 추가되어 대규모 AI 및 시뮬레이션 환경에 적합합니다.

### [AKS Pod CIDR 대역 확장](https://azure.microsoft.com/updates?id=557907)
AKS 클러스터 내에서 Pod IP 대역을 유연하게 증설, 클러스터 재생성 없이도 손쉽게 워크로드 확장이 가능합니다.

### [Azure Database for PostgreSQL – PgBouncer 1.25.1 정식 지원](https://azure.microsoft.com/updates?id=559623)
커넥션 풀링이 내장되어 대용량 트랜잭션 환경에서 연결 효율과 신뢰성이 획기적으로 높아집니다.


## 🚀 관리 & 보안 & 네트워킹 기능 강화

최근 Azure의 네트워크·보안 및 관리 기능은 더욱 체계화되었습니다. Azure Service Bus의 NSP(Network Security Perimeter) 정식 지원으로 PaaS 리소스 간 중앙 집중 방식의 접근제어가 구현되며, 운영 환경에 대한 감사 및 규정 준수가 쉬워졌습니다. AKS의 네임스페이스·워크로드 관측성 강화로 실시간 장애 진단 및 리소스 사용량 분석이 용이해졌고, Azure Network Watcher에서 보안 규칙 영향도 분석(미리 보기)으로 위협 대응과 장애 예방이 효율화됐습니다. 전체적으로 보안 체계 강화와 운영 편의성 향상이 돋보입니다.

### [Azure Service Bus용 Network Security Perimeter 정식 지원](https://azure.microsoft.com/updates?id=559899)
네트워크 보안 경계 설정으로, PaaS 리소스 간 외부 노출 차단 및 보안 통신 환경을 중앙집중형 제어 방식으로 제공합니다.

### [AKS 네임스페이스 및 워크로드 뷰 관측성 강화](https://azure.microsoft.com/updates?id=560039)
Azure Monitor와 통합되어 클러스터·파드 상태, 장애 원인, 리소스 사용량 등을 실시간으로 모니터링할 수 있습니다.

### [Azure Network Watcher의 규칙 영향 분석 기능(미리 보기)](https://azure.microsoft.com/updates?id=559876)
보안 규칙 적용 전 영향도 예측, 충돌 방지, 네트워크 안정성 확보로 장애 가능성을 사전에 관리할 수 있습니다.


## 🛠️ 개발자 생산성 & 데이터 마이그레이션

데이터 마이그레이션, 데이터 복구, 개발 자동화 및 생산성 개선 기능이 주요 업데이트로 배포되었습니다. Azure Functions는 MCP 리소스 트리거를 지원하여 더욱 인터랙티브한 앱 구현이 가능해졌고, Azure Migrate는 Azure Files 평가 기능(미리 보기)으로 SMB 및 NFS 파일의 클라우드 이관을 구조적으로 지원합니다. PostgreSQL 유지보수 알림, 아이템 리커버리, 마이그레이션 도우미 등 다양한 진단·복구·이관 도구들이 개발자 경험을 크게 높였습니다.

### [Azure Functions의 MCP 리소스 트리거 지원](https://azure.microsoft.com/updates?id=559981)
Functions 기반 MCP 서버에서 리소스를 직접 노출하여 동적 파일 및 UI 컨텐츠를 유연하게 제공할 수 있습니다.

### [Azure Migrate: Azure Files 평가 기능(미리 보기)](https://azure.microsoft.com/updates?id=560025)
온프레미스 파일 서비스의 마이그레이션에 필요한 용량 산정, 비용 분석, 최적 SKU 추천 등 사전 진단 기능을 강화했습니다.

### [Azure Service Health의 지역 단위 유지보수 알림 통합](https://azure.microsoft.com/updates?id=559628)
PostgreSQL 서버 기반의 유지보수 알림이 지역 단위로 통합 관리되어 업무 협업 및 계획 수립이 더욱 용이해집니다.
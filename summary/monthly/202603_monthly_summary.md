# Azure 월간 업데이트 요약 - 2026년 03월

## 전반적인 트렌드와 핵심 인사이트

2026년 3월 Azure 업데이트는 AI와 데이터 플랫폼의 대규모 혁신과 기업 환경 중심의 기능 강화가 두드러집니다. 특히 Microsoft Foundry와 Microsoft Fabric 중심의 업데이트가 대량으로 이루어졌으며, 실무 환경에 바로 적용 가능한 정식 지원(General Availability) 기능이 여럿 추가되었습니다. Foundry Agent Service의 정식 출시, GPT-5.4와 Grok 4.1 등 첨단 AI 모델의 GA, 산업별 특화 분석/실시간 데이터 처리, 엔터프라이즈용 보안 및 네트워크 기능 확대 등이 주요 변화로 꼽힙니다.

이번 달은 AI 모델 운영의 품질 관리 및 자동화, 실제 기업 환경의 수요에 맞춘 확장성·관찰성(Observability) 강화, 미리 보기 기능을 통한 실험적 혁신이 활발하게 이루어진 점이 인상적입니다. 데이터 이동과 통합의 자동화, 여러 클라우드와 온프레미스 환경을 실무에서 손쉽게 연결할 수 있게 한 점 역시 사용성과 효율성에서 큰 진전으로 평가됩니다.

보안 분야에서는 네트워크 격리, 프라이빗 링크, CMK(고객 관리 키) 등 조직별 데이터 보호와 컴플라이언스 대응력 강화가 강하게 반영됐습니다. DevOps 및 관리 자동화, 인프라 모빌리티, 배포 파이프라인 간소화 등 운영 측면의 개선도 지속적으로 이루어지고 있습니다.

AI와 데이터 기능뿐 아니라, 컨테이너, VM, Storage, 네트워크, 관리 자동화 등 전통적 Azure 서비스들도 신기능 추가와 서비스 지원 종료(retirement)에 대한 적극적인 공지와 마이그레이션 가이드가 제공되었습니다. 이는 고객의 장기적인 기술 전략과 운영 안정성에 기여할 수 있는 변화입니다.

이번 달은 “실질적 운영환경에서 AI와 데이터 기반 혁신을 구현한다”라는 Microsoft의 전략이 구체적이고 다층적으로 추진되는 한 달로 평가됩니다.


## 카테고리별 업데이트

---

## 🧠 Microsoft Foundry

이번 달 Foundry는 AI 에이전트의 기업 적용을 위한 실무적 기능이 정식 지원으로 대거 출시되었습니다. 특히 Foundry Agent Service의 GA와 Voice Live, 평가·감시·추적 기능의 GA, 다양한 최신 AI 모델(GPT-5.4, Grok, NVIDIA Nemotron 등)의 지원이 핵심입니다. 책임 있는 AI, 보안, 실시간 음성·다중모달 지원 등 기업의 실제 운영 요구에 맞는 확장성과 품질 관리가 강조되고 있습니다.

### [Foundry Agent Service 정식 지원: 엔터프라이즈급 보안/관찰성/실시간 음성](https://devblogs.microsoft.com/foundry/foundry-agent-service-ga/)
- 엔터프라이즈급 AI 에이전트 플랫폼 출시, 프라이빗 네트워킹, 실시간 음성, 철저한 평가와 관찰성 기능 제공.

### [GPT-5.4와 GPT-5.4 Pro 정식 지원](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/introducing-gpt-5-4-in-microsoft-foundry/ba-p/4499785)
- 최신 고급 AI 모델 GA, 도구 통합·장기 맥락·실행 신뢰성·생성물 품질 등 업무 환경 최적화.

### [Voice Live 기반 음성 네이티브 에이전트 미리 보기](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/public-preview-voice-native-agents-in-microsoft-foundry/ba-p/4502756)
- 실시간 음성 대화 에이전트 개발환경 지원, 다국어·멀티모달·엔터프라이즈 보안 및 트래픽 품질 평가.

### [AI 에이전트 운영 품질 평가·감시·추적 기능 정식 지원 및 OpenTelemetry 연계](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/generally-available-evaluations-monitoring-and-tracing-in/ba-p/4502760)
- 평가/감시/추적 기능 GA, Azure Monitor·Grafana 연동, 자동화 CI/CD 품질 게이트.

### [Fireworks AI 통합 및 커스텀 모델 임포트 미리 보기](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/announcing-fireworks-ai-on-microsoft-foundry/ba-p/4500950)
- 고성능 커스텀 오픈소스 AI 모델의 서버리스 인퍼런스 지원, 생산 환경 맞춤 커스텀 모델 배포 실험 가능.

---

## 📊 Microsoft Fabric

Fabric은 AI 조직을 위한 데이터 준비, 확대된 보안, 네트워크 설정, 애널리틱스/대시보드 실시간화까지 다양한 부문에서 정식 지원 기능을 내놓았습니다. ADF/Synapse, 온프레미스 게이트웨이, 자동화 연계 등 데이터 통합과 운영 자동화의 접근성을 크게 높였습니다. Preview 기능도 실시간 이벤트 처리, 다중모달 AI 등 향후 혁신 방향성이 뚜렷합니다.

### [Tonic Textual로 비정형 데이터 AI 준비 지원 (GA)](https://blog.fabric.microsoft.com/en-US/blog/from-restricted-to-ai-ready-preparing-unstructured-data-directly-in-microsoft-fabric-with-tonic-textual-generally-available/)
- 비정형 데이터에서 AI 활용도를 높일 수 있는 데이터 준비 기능 정식 출시.

### [비즈니스 이벤트 기능/실시간 애플리케이션 미리 보기](https://roadmap.fabric.microsoft.com/?product=real-timeintelligence)
- Fabric 기반 실시간 이벤트 기반 업무 자동화 기능 preview 출시.

### [온프레미스 데이터 게이트웨이 자동 업데이트(GA)](https://blog.fabric.microsoft.com/en-US/blog/on-premises-data-gateway-auto-update-admin-triggered-generally-available/)
- 온프레미스 원격 데이터 연동의 관리 자동화 기능.

### [워크스페이스 태그로 빠른 검색 및 콘텐츠 관리(GA)](https://blog.fabric.microsoft.com/en-US/blog/find-and-manage-workspaces-faster-with-workspace-tags-generally-available/)
- 워크스페이스별 메타데이터 태깅으로 데이터 관리 향상.

### [SQL Server Management Studio(SSMS)·GitHub Copilot 연계(GA)](https://blog.fabric.microsoft.com/en-US/blog/sql-server-management-studio-ssms-22-4-1-and-github-copilot-in-ssms-generally-available/)
- 친화적 AI 코드 지원·자동화·테스트 기능 등 개발 환경 개선.

---

## 🛡️ 보안·네트워크·관리

이번 달에는 네트워크 격리, IP Firewall, CMK(고객 관리 키), VNET·프라이빗 링크 지원 등 엔터프라이즈 데이터 보호 및 거버넌스 관련 기능이 대거 정식 지원으로 추가됐습니다. Azure Firewall, WAF, 컨테이너·네트워크 관리도 서비스 정책·운영 편의성 강화. 퇴역(retirement) 관련 공지도 운영자 관점에서 중요한 참고 정보입니다.

### [IP Firewall 룰 및 프라이빗 링크 지원](https://blog.fabric.microsoft.com/en-US/blog/workspace-level-ip-firewall-rules-in-microsoft-fabric-generally-available/)
- Fabric 워크스페이스별 접근 차단 정책 직접 설정 가능.

### [CMK 기능 추가: Fabric SQL DB에서 직접 관리](https://blog.fabric.microsoft.com/en-US/blog/customer-managed-keys-cmk-in-fabric-sql-database-generally-available/)
- 조직별 키 관리로 데이터 보안과 규제 대응력 개선.

### [VNET Data Gateway 인증서 및 프록시 지원(GA)](https://blog.fabric.microsoft.com/en-US/blog/certificate-and-proxy-support-for-vnet-data-gateway-generally-available/)
- 엔터프라이즈 환경에서 강한 네트워크 보안 옵션 강화.

### [Azure Firewall Draft & Deploy 기능(GA)](https://azure.microsoft.com/updates?id=558072)
- 정책 변경 시 실시간 적용 병행, 배포 효율성 대폭 향상.

### [Azure Web Application Firewall DRS 2.2 규칙 지원 정책 변경](https://azure.microsoft.com/updates?id=558016)
- WAF 관리 규칙 세트 수명/업데이트 주기 명확화, 지원 종료 일정 사전 안내.

---

## 💡 데이터·분석·DevOps

Azure SQL, Databricks, PostgreSQL 등 데이터베이스 서비스에서 GA 및 미리 보기 업데이트가 다양하게 출시되었습니다. 자동 인덱스 최적화, Hyperscale 확장, 다양한 마이그레이션 경로, 데이터 이동 자동화, DevOps/CI/CD 연계, 프로파일링 및 쿼리 최적화 등 기업 데이터 환경 운영 효율성 강화가 두드러집니다. 또한 운영 자동화(Azure Monitor, Prometheus)와 Spot/Low-Priority VM 마이그레이션 등 DevOps 개선도 눈에 띕니다.

### [Azure SQL Database 정식 지원 및 관리 키, 자동 인덱싱/확장, 마이그레이션 등 신기능](https://azure.microsoft.com/updates?id=558121)
- SQL 프로젝트/쿼리 개선, Hyperscale 시리즈 확장, 업그레이드/보안 강화.

### [Azure Databricks Lakebase 정식 지원](https://azure.microsoft.com/updates?id=557991)
- OLTP 및 분석 데이터 통합, AI 에이전트 활용 최적화.

### [Databricks Workspace 네트워크 설정 및 Lakeflow Connect 무료 티어](https://azure.microsoft.com/updates?id=558810)
- Workspace 네트워크 직접 관리, 데이터 인입 비용효율적 활용.

### [Postgresql/EBD/AlloyDB 등 마이그레이션 신기능](https://azure.microsoft.com/updates?id=558865)
- 엔터프라이즈 전환시 데이터 이동/마이그레이션의 안정성·효율성 증대.

### [Azure Monitor Prometheus 추천 알림 및 Log Analytics 요약 rules 개선](https://azure.microsoft.com/updates?id=558825)
- 모니터링/프로메테우스 자동화, 데이터 요약 규칙 실패 자동 재시도.

---

## 🤖 AI·모델 운영·음성/멀티모달

Azure AI Service 및 Microsoft Foundry를 활용한 최신 LLM, 음성 합성, 모델 평가/운영 측면의 발전이 집중적으로 이루어졌습니다. Neural HD TTS, VibeVoice ASR 등 AI 기반 음성 합성·인식 모델의 품질 향상과 지역 커버리지 확대가 두드러지며, 다양한 모델의 GA, 커스텀 모델 운영, 운영간 품질 평가 및 관찰성 기능이 실무에서 바로 사용될 수 있는 수준에 도달했습니다.

### [Azure Speech Neural HD 음성합성 2.5 업데이트 (GA)](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/azure-speech-neural-hd-text-to-speech-recent-voice-updates/ba-p/4505380)
- 자연스러운 억양, 다중 스타일, 다국어 커버리지, 가격 인하.

### [Microsoft Foundry 기반 VibeVoice ASR 연속 음성 인식 모델(GA)](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/introducing-vibevoice-asr-longform-structured-speech-recognition/ba-p/4501276)
- 최대 60분 연속 음성 인식, 화자 구분/타임스탬프, 멀티언어 코드스위칭/실시간 대응.

### [AI 평가/관찰성 및 책임있는 AI 관리 강화 (GA)](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/generally-available-evaluations-monitoring-and-tracing-in/ba-p/4502760)
- LLM 자동 평가, Azure Monitor 연동, 품질 기준 자동화/실시간 추적.

### [Grok 4.0 GA 및 Grok 4.1 Fast 모델 출시](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/grok-4-0-goes-ga-in-microsoft-foundry-and-grok-4-1-fast-arrives/ba-p/4497964)
- 다중모델 추론, 속도/확장성/안전성 보증, 다양한 엔터프라이즈 AI 경험 지원.

### [NVIDIA Nemotron/NIM, IBM Granite, Sarvam 등 최신 AI 모델 GA](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/now-in-foundry-nvidia-nemotron-3-super-120b-a12b-ibm-granite-4-0/ba-p/4506917)
- 장문 맥락/이중모델/추론, 멀티언어/음성 처리, 엔터프라이즈급 배포 지원.

---

## 🔗 컨테이너·VM·스토리지·운영 자동화

AKS, VM, 스토리지 등 인프라/컨테이너 영역에서는 네트워크/운영 감시, GPU/스토리지 성능 개선, 지원 종료 VM/OS에 대한 마이그레이션 권장, 프리뷰 기능으로 운영 효율성·보안 강화에 초점을 맞추었습니다. 최신 컨테이너 네트워크 감시, 모니터링, 실시간 알림, VM/Batch 마이그레이션, 스토리지 이동 자동화 등이 운영 안정성을 높이는 움직임입니다.

### [AKS 컨테이너 네트워크 로그/메트릭 필터링 정식 지원](https://azure.microsoft.com/updates?id=557892)
- 네트워크 트래픽 실시간 분석 및 장애 진단.

### [Azure Premium SSD v2 South India 지역 GA](https://azure.microsoft.com/updates?id=559526)
- 최신 스토리지 지역별 확장, IO 성능 강화.

### [Azure Sphere, VM, Batch 등 서비스 지원 종료(퇴역) 안내](https://azure.microsoft.com/updates?id=557123)
- AV36P/AV52, HBv2, NP, HC 계열 VM 및 Windows Server 2016 등 장기 지원 종료 일정 공지.

### [Ephemeral OS Disk, GPU/네트워크/클러스터 관리 프리뷰](https://azure.microsoft.com/updates?id=559322)
- VM/VMSS 성능 향상, 운영 신속성 및 안정성 강화.

### [Azure Storage Mover, AWS S3-Blob 프라이빗 데이터 이동 프리뷰](https://azure.microsoft.com/updates?id=558651)
- 멀티클라우드 데이터 이동을 자동화·보안 강화.

---

## 🗃️ 마이그레이션·지원 종료(retirement)·특별 공지

이번 달은 장기 지원 종료(retirement) 및 마이그레이션 정책에 대한 명확한 안내가 다수 이루어졌습니다. Cosmos DB for PostgreSQL, AV36P/AV52, Windows Server 2016 Marketplace 이미지, Azure Sphere, Batch Low-Priority VM 등 다양한 서비스가 향후 수년에 걸쳐 순차적으로 지원 종료/대체됨을 공지하고, 전환 가이드와 마이그레이션 도구를 안내합니다. 이를 통해 고객의 운영 안정성, 장기 기술 전략 수립에 도움이 될 수 있습니다.

### [Azure Cosmos DB for PostgreSQL, 2029년 3월 지원 종료 안내](https://azure.microsoft.com/updates?id=556085)
- PostgreSQL Elastic Cluster로 이전 권장, 데이터 이동 실무 가이드 제공.

### [Azure Sphere 2031년 지원 종료, Azure IoT 대체 포함](https://azure.microsoft.com/updates?id=557123)
- IoT 서비스 전략 전환, 하드웨어/라이선스 매입 일정 안내, 대체 솔루션 안내.

### [AV36P/AV52, HBv2, NP, HC 계열 VM 2027~2029년 지원 종료](https://azure.microsoft.com/updates?id=557094)
- VM 유형별 단계적 지원 종료/이동 가이드 강화.

### [Emissions Impact Dashboard for Azure 2027년 지원 종료](https://azure.microsoft.com/updates?id=558278)
- 신규 Carbon Optimizer 솔루션으로 전환 유도.

### [Azure Policy 빠른 적용 및 Login/Logout workaround 은퇴](https://azure.microsoft.com/updates?id=558102)
- 정책 적용 성능 개선, 기존 수동 워크어라운드 폐기.

---

## 총평 및 다음 달 전망

3월 Azure 업데이트는 AI 에이전트의 실제 운영환경 구현, 데이터 보호·거버넌스 강화, 운영 자동화, 그리고 최신 인프라 마이그레이션 지원에 집중된 전략적 변화를 보여줍니다. Microsoft Foundry와 Fabric의 정식 지원 기능 확대는 AI와 데이터 기반 혁신을 실무에 단숨에 적용할 수 있게 하였으며, 평가·관찰성·운영 효율·보안 등 장기적인 품질 관리를 위한 인프라적 기반도 견고하게 마련되었습니다.

개발자와 데이터 관리자, AI·운영 전문가 모두에게 실무적 가치가 높은 기능이 정식 지원되었고, 미리 보기 기능은 데이터 처리·AI 적용·자동화 방식의 미래를 제시하며 업계 혁신을 이끌고 있습니다. 지원 종료(retirement) 정책은 앞으로의 기술 전략 수립과 안정적 전환을 위한 명확한 가이드를 제공합니다.

다음 달은 AI 기반 자동화·보안·모델 운영 분야 추가 혁신, Fabric과 Foundry 플랫폼의 기능 확장, 실시간 데이터 처리/모니터링·배포 자동화 영역에서 더 다양한 기능이 나오며, 리전·서비스 확장, 각종 미리 보기 기능의 정식 지원 전환이 기대됩니다. Azure 는 실제 서비스 운영에 필수적인 품질, 보안, 자동화, 효율성의 기준을 끊임없이 높여갈 것입니다.
# Azure 월간 업데이트 요약 - 2026년 03월

## 전반적인 트렌드와 핵심 인사이트

2026년 3월 Azure 업데이트는 인프라 혁신과 AI 플랫폼 고도화가 동시에 진행되는 “모범 사례와 신기술의 융합”이 핵심 트렌드입니다. 전통적으로 강한 Azure 인프라 서비스에는 최신 관리 및 네트워크 기능, 데이터 통합 자동화, 신형 스토리지 옵션이 추가되어 엔터프라이즈급 확장성과 보안이 한층 강화되었습니다. 특히 네트워크 관리 기능(예: Azure Firewall Draft & Deploy, Web Application Firewall DRS 2.2 등), 프리미엄 SSD v2의 지역 확장, 컨테이너 네트워크 로그 등 실무 중심의 기능 개선이 눈에 띕니다.

데이터베이스 측면에서는 Azure SQL, PostgreSQL, Databricks의 운영 자동화, 관측성 및 마이그레이션 편의성이 크게 개선되었습니다. AWS-데이터 이전 자동화, pgoutput 활용 등 멀티클라우드 연동 지원이 확대되고, SQL 프로젝트 기반 DevOps의 본격화로 데이터 개발과 CI/CD가 긴밀하게 연결되었습니다.

AI 및 Microsoft Foundry/Microsoft Fabric 분야에서는 확실한 대세 전환이 감지됩니다. Microsoft Foundry는 GPT-5.4, Grok 등 신형 AI 모델의 출시와 함께, 엔터프라이즈 실무를 염두에 둔 고도화된 에이전트 분석·운영 기능(GA 평가, 추적, 모니터링) 및 실시간 음성 기반 AI 에이전트 지원이 정식 출시되었습니다. 파운드리와 퍼브릭은 데이터 영역 전반으로 확장된 모듈형 배포와 평가체계, 고도화된 보안(Private Link, BYO VNet 등), 관측성(Workspace Monitoring)과 같은 체계적 운영관리 옵션을 제공하며, 단순 PoC 단계에서 실제 대규모 운영까지 성장 가능한 구조를 제시합니다.

또한 데이터플로우/파이프라인 자동화, 미러링, 이벤트 기반 워크로드, 실시간 추론 및 모니터링, 다양한 시스템 간의 연결성 보장 등 Fabric을 중심으로 전방위 데이터 통합과 AI 실무화가 빠르게 진행되고 있습니다. 기존 Synapse 및 데이터팩토리 파이프라인을 손쉽게 마이그레이션할 수 있는 지원 역시 대규모 현대화 전략의 큰 촉진제가 될 전망입니다.

마지막으로, 관리 자동화와 보안 강화, 다중 클라우드 및 하이브리드 연동, 생산성 중심 UI/UX 개선, 더 넓게는 다양한 VM 시리즈 및 운영체제의 사용 종료와 마이그레이션 절차까지 실제 엔터프라이즈 현장에 필수적인 “서비스 책임성과 미래지향적 전환”의 메시지가 뚜렷하게 나타나고 있습니다.

---

## 🧠 Microsoft Foundry

이번 달 Foundry 카테고리에서는 엔터프라이즈 AI 실무화를 위한 모델 관리, 평가, 배포 자동화, 보안 및 관측성의 통합이 주목됩니다. 새로운 AI 모델(GPT-5.4, Grok, VibeVoice 등) 출시와 음성 기반 에이전트, 실시간 평가·모니터링, 프리미엄 배포옵션, 다양한 오픈모델의 통합 등 기업의 AI 업무 환경을 위한 체계적 운영 솔루션이 정식 지원되었습니다.

### [GPT-5.4 모델 정식 지원](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/introducing-gpt-5-4-in-microsoft-foundry/ba-p/4499785)
GPT-5.4, GPT-5.4 Pro, 미니/나노 모델 등 실무 환경에 최적화된 신형 AI 모델이 Foundry에 정식 지원되었습니다. 복잡한 이유 추론, 멀티에이전트 워크플로우, 고도 분석 등 엔터프라이즈 전용 기능이 강화됐으며, 실시간/분류/추론 시나리오별 다양한 모델 선택과 비용 최적화가 가능합니다.

### [Foundry Agent Service 정식 지원 및 음성 라이브 공개](https://devblogs.microsoft.com/foundry/foundry-agent-service-ga/)
진화된 Foundry Agent Service가 정식 지원(GA)되며, Voice Live와 프라이빗 네트워킹, 고품질 평가·모니터링 등 다양한 기능이 통합되었습니다. 실시간 음성 기반 AI 에이전트 개발이 급격히 용이해졌으며, 엔터프라이즈 보안과 평가체계 역시 기본 제공됩니다.

### [AI 에이전트 평가, 모니터링 및 추적 정식 지원](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/generally-available-evaluations-monitoring-and-tracing-in/ba-p/4502760)
Foundry Control Plane와 Azure Monitor 연동을 통해 에이전트 품질 모니터링, 실시간 평가, 트레이스 분석이 일원화되었습니다. 기업 운영 환경에서 안전, 품질, 성능의 지속적 개선이 가능해지며, CI/CD 파이프라인과 연계한 품질 게이트를 쉽게 적용할 수 있습니다.

### [VibeVoice ASR 및 다수 신규 모델 배포](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/introducing-vibevoice-asr-longform-structured-speech-recognition/ba-p/4501276)
장시간 음성 인식, 화자 구분, 멀티언어 지원 등 VibeVoice ASR을 비롯한 다수 신규 모델이 파운드리 및 Hugging Face 연동으로 배포되었습니다. 생산성 향상, 대규모 음성 처리 및 엔터프라이즈 특화 시나리오에 최적화된 기능이 제공됩니다.

### [우수 사례: AI 에이전트의 시뮬레이션 기반 평가 및 개선](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/how-veris-ai-and-lume-security-built-a-self-improving-ai-agent/ba-p/4504424)
실제 운영 실패 시나리오를 자동으로 시뮬레이션·분석하고, Reinforcement Learning과 프롬프트 자동 최적화로 에이전트 품질을 40% 이상 개선한 사례 발표. Foundry 기반 자동 평가, 최적화 루프, 보안·컴플라이언스 통합의 실제 성공 전략이 제시되었습니다.

---

## 🧩 Microsoft Fabric

Fabric 업데이트는 데이터·AI 기반 실무 체계의 구축과 자동화, 워크로드 확장, 멀티환경 통합, ISV/파트너 생태계 강화가 핵심입니다. 데이터통합, 파이프라인 현대화, 실시간 이벤트 기반 데이터 처리, 확장성·보안·운영 관리 기법이 대폭 추가되었습니다.

### [AI Ready: 미러링, Data Factory, 실시간 이벤트 기반 기능 강화](https://blog.fabric.microsoft.com/en-US/blog/fabric-data-factory-at-fabcon-atlanta-built-for-modern-data-integration/)
Data Factory, 미러링, Eventstreams, 실시간 처리, CDC 연동 등 Fabric 내 데이터 통합·이동 기능이 대폭 강화되어 이기종 데이터/운영환경 통합이 쉽고 빠르게 가능해졌습니다.

### [파트너·ISV 생태계 확장 및 워크로드 관리](https://blog.fabric.microsoft.com/en-US/blog/the-power-of-the-microsoft-fabric-ecosystem-isvs-building-natively-on-fabric/)
ISV 전용 워크로드 관리, 파트너 솔루션 배포체계, 자동화된 확장 관리 등 Fabric을 통한 맞춤형 솔루션 구축/운영 방식이 정식 지원되어 생태계 혁신을 촉진합니다.

### [실시간 인텔리전스 및 운영시스템 통합](https://blog.fabric.microsoft.com/en-US/blog/industrial-analytics-delivered-at-scale-powered-by-fabric-real-time-intelligence-and-fusion-data-hub/)
실시간 공정 데이터 분석, 산업 IoT, 실시간 KPI 모니터링을 위한 데이터 허브/지능 플랫폼이 Fabric 기반으로 통합 제공되어 제조·운영현장의 실질적 혁신을 뒷받침합니다.

### [워크스페이스 모니터링 및 대시보드 표준화](https://blog.fabric.microsoft.com/en-US/blog/workspace-monitoring-dashboard-templates-in-microsoft-fabric-eventhouse/)
Workspace Monitoring 대시보드, 텔레메트리 자동화, 이벤트하우스 기반 대시보드 템플릿 등 Fabric 내 데이터 및 작업관리의 표준화·자동화 기능이 확장되었습니다.

### [데이터플로우 Gen2, 유연한 변수 라이브러리와 진단 도구 추가](https://blog.fabric.microsoft.com/en-US/blog/dataflow-gen2-variable-library-integration-in-microsoft-fabric-generally-available/)
Dataflow Gen2에 변수 라이브러리 통합, CI/CD 및 ALM 지원, 데이터플로우 진단 도구 등 실무 대규모 환경에 맞는 운영 및 관리 도구가 정식 지원되어 데이터 통합·자동화 관리의 효율성이 개선되었습니다.

---

## ⚙️ Azure 인프라 및 컴퓨팅 서비스

기존 Azure 인프라 서비스에는 스토리지·VM·네트워킹의 성능 최적화, 관리 자동화, 지역 지원 확대, VM 시리즈의 사용 종료 및 마이그레이션 안내 등 엔터프라이즈 운영 책임성이 명확해지는 변화가 이뤄졌습니다.

### [Azure Premium SSD v2, South India 지역 출시](https://azure.microsoft.com/updates?id=559526)
프리미엄 SSD v2가 South India 지역에 정식 지원되며, SQL Server, SAP, 대규모 빅데이터·분석 등 핵심 워크로드의 저지연·고성능·저비용 스토리지 옵션이 확대되었습니다.

### [Azure Container Storage v2.1.0 – Elastic SAN 통합](https://azure.microsoft.com/updates?id=557912)
Kubernetes/컨테이너 환경에서 Elastic SAN 연동으로 가변적 저장소 관리, 중앙제어, 성능 및 활용률 최적화가 가능해졌습니다.

### [Azure Monitor Prometheus, Arc-enabled Kubernetes 권장 알림](https://azure.microsoft.com/updates?id=558825)
Prometheus 커뮤니티 권장 알림을 Arc-enabled Kubernetes에 원클릭 활성화, 클러스터/노드/포드 수준의 실시간 장애 대응 및 CI/CD 자동화 연동이 가능해졌습니다.

### [Azure Red Hat OpenShift, 인도네시아 중앙 지역 지원 및 관리 ID 기능 확대](https://azure.microsoft.com/updates?id=559552)
Azure Red Hat OpenShift가 인도네시아 중앙에서 정식 지원되며, 관리된 신원 및 워크로드 ID 기능이 추가되어 공공·규제 환경에서 보안 요건을 충족합니다.

### [VM/Machine 시리즈 사용 종료 안내 및 마이그레이션 가이드](https://azure.microsoft.com/updates?id=548525)
HBv2, HC, NP 등 VM 시리즈가 2027년 사용 종료 예정임을 알리고, 최신 HPC VM으로의 마이그레이션을 권장하고 있습니다. Batch, Windows Server 2016 Marketplace 등 다양한 OS/플랫폼의 종료 시기 및 대처 방안도 안내합니다.

---

## 💡 데이터베이스 & 관리 자동화

데이터베이스는 Azure SQL, PostgreSQL, Databricks 등 다양한 플랫폼에서 관리 자동화, DevOps, 마이그레이션 지원, 실제 운영자 중심 편의 기능이 크게 확장되었습니다.

### [Azure SQL Database, SSMS와 GitHub Copilot 혁신적 연동](https://azure.microsoft.com/updates?id=558134)
GitHub Copilot을 SSMS에 통합, 자연어 기반 SQL 코드 생성·수정·최적화가 가능하며, 개발자의 생산성과 협업 능력이 크게 향상됩니다.

### [Databricks Lakebase 및 네트워크 구성 유연화](https://azure.microsoft.com/updates?id=557991)
Databricks Lakebase가 정식 지원되고, VNet 관리시 유연한 전환/설정이 가능해져 데이터분석·ML 환경의 확장성과 보안이 강화되었습니다.

### [Terraform/Bicep/Ansible 기반 PostgreSQL Elastic Cluster 자동화](https://azure.microsoft.com/updates?id=558145)
클러스터 프로비저닝·확장·관리 자동화가 각종 IaC도구(Terraform, Bicep, Ansible)로 지원되어 배포관리의 일관성과 신속성이 극대화되었습니다.

### [pgoutput 플러그인 및 AlloyDB/EDB 원천 마이그레이션 지원](https://azure.microsoft.com/updates?id=558846)
PostgreSQL 온라인 마이그레이션에서 native pgoutput 지원, AlloyDB, EDB 등 다양한 오픈소스 환경에서 Azure로의 신속한 원천 마이그레이션이 가능해졌습니다.

### [Azure SQL Managed Instance, 실시간 변경 이벤트 스트리밍 지원](https://azure.microsoft.com/updates?id=558884)
Azure SQL MI에서 트랜잭션 커밋 이벤트를 Azure Event Hubs로 실시간 스트리밍, CDC 없이 운영/분석 플랫폼 실시간 연동이 가능해졌습니다.

---

## 🔒 네트워킹 및 보안

네트워크 및 보안 서비스는 방화벽 및 WAF 관리 강화, Private Link/프라이빗 엔드포인트 확대, 관리형 키 사용, 규제 산업 대응 등 보안의 일관성과 자동화가 핵심입니다.

### [Azure Firewall Draft & Deploy – 정책 관리 혁신](https://azure.microsoft.com/updates?id=558072)
정책 변경을 드래프트로 준비, 일괄 배포하는 2단계 방식이 도입되어 실운영환경의 장애 리스크와 배포 시간 감소를 실현합니다.

### [Web Application Firewall DRS 2.2, 규칙 Lifecycle 명확화](https://azure.microsoft.com/updates?id=558016)
최신 규칙셋 지원 정책 및 Lifecycle(최신 3개 버전만 지원, 정책 자동 관리) 명확화로 보안 업데이트 일관성과 엔터프라이즈 보안 책임 강화.

### [Cosmos DB Mirroring, 프라이빗 엔드포인트 지원](https://azure.microsoft.com/updates?id=558836)
미러링 데이터의 프라이빗 네트워크 격리, 네트워크 권한통제, 규제 산업에서의 보안 요건 충족 등 보안 중심 데이터 이동의 강화.

### [Azure SQL Database, 버전 없는 투명 암호화 키 지원](https://azure.microsoft.com/updates?id=558183)
TDE 구성시 버전 없는 키 URI 지원, 키 버전 관리/교체 및 연계운영의 손쉬운 자동화와 안정성 확보.

### [Azure Blob Storage Entra ID 기반 SFTP 연동 (미리보기)](https://azure.microsoft.com/updates?id=558662)
Entra ID 기반 SFTP 접속 지원, MFA/조건부 접근/외부 계정 연동, RBAC 자동 연계 기능 등 현대적 보안·운영 환경 구현.

---

## 🌐 미리 보기/신제품/실험적 기능

본 카테고리는 Azure 및 Fabric에서 미리 보기(Public Preview)로 출시된 신규 기능과 실험적 솔루션을 다루며, 차기 대규모 운영환경을 위한 실질적 혁신 요소들이 등장했습니다.

### [Fabric AI 기능 멀티모달 지원 및 이미지/PDF 추론](https://blog.fabric.microsoft.com/en-US/blog/unlock-insights-from-images-and-pdfs-with-multimodal-support-in-fabric-ai-functions-preview/)
Notebooks, pandas/Spark 환경에서 이미지, PDF 등 비정형 데이터에 AI 기능(분류, 요약, 감정분석) 통합. 데이터 사이언스 실무 편의성 대폭 개선.

### [파운드리 음성 네이티브 에이전트, 실시간 대화/동작 지원(공개 미리보기)](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/public-preview-voice-native-agents-in-microsoft-foundry/ba-p/4502756)
음성 기반 실시간 AI 에이전트 개발 지원, Voice Live API로 140개 언어·700개 음성, 자연스러운 대화 및 다양한 산업 시나리오 즉시 적용.

### [Azure Monitor, OpenTelemetry Collector 및 OTLP 데이터 수집 지원(미리보기)](https://azure.microsoft.com/updates?id=559273)
OpenTelemetry Collector와 직접연동, OTLP 로그/트레이스/메트릭 수집, PromQL 질의·알림, 로깅/모니터링/합성까지 클라우드 네이티브 운영 환경 유기화.

### [Azure Storage Mover, AWS S3 Private 네트워크 데이터 마이그레이션(미리보기)](https://azure.microsoft.com/updates?id=558651)
AWS S3 Private VPC에서 Azure Blob으로 직접 데이터 이동, 보안/컴플라이언스·자동화 관리·실시간 모니터링까지 멀티클라우드 운영 편의성 확대.

### [Power Query API, 프로그램적 데이터 변환(Preview)](https://blog.fabric.microsoft.com/en-US/blog/execute-power-query-programmatically-in-microsoft-fabric/)
Power Query를 API로 직접 호출, 자동화된 데이터 변환·품질관리·데이터 엔지니어링 워크로드 일원화가 가능해졌습니다.

---

## 📣 서비스 사용 종료 및 리타이어먼트

이번 달에도 다양한 서비스/VM 시리즈/운영체제의 사용 종료 및 마이그레이션 정보가 공지되었습니다. 대규모 데이터 현장과 인프라 현대화 프로젝트에 꼭 필요한 사전 준비와 대처 전략이 명확히 제시됩니다.

### [Cosmos DB for PostgreSQL 지원 종료 안내](https://azure.microsoft.com/updates?id=556085)
2029년 3월 31일, Cosmos DB for PostgreSQL 서비스 지원 종료 예정. Elastic Cluster로 무중단 마이그레이션 권장.

### [Azure Sphere, 2031년 7월 31일 서비스 종료 예정](https://azure.microsoft.com/updates?id=557123)
마이크로컨트롤러 보안 플랫폼 Azure Sphere, 하드웨어 리디자인 및 Azure IoT, 3rd Party 대안 검토 필요.

### [Batch Low-Priority VM, Spot VM 자동 마이그레이션](https://azure.microsoft.com/updates?id=543279)
2026년 3월, Batch Low-Priority VM이 Spot VM으로 시스템 전환 및 과금, 기존 API 연동 구조 자동 대응.

### [VM/Marketplace 이미지, OS 종료 일정 안내 및 대체 가이드](https://azure.microsoft.com/updates?id=549077)
Windows Server 2016 Marketplace 이미지 2027년 1월 12일 지원 종료, 최신 Windows Server 또는 커스텀 이미지 마이그레이션 권장.

### [Prometheus Sidecar for remote-write 사용 중단(2027년 3월 31일)](https://azure.microsoft.com/updates?id=550519)
Prometheus remote-write sidecar가 사용 중단되어, 직접 remote-write 설정으로 변경 필요.

---

## 🏢 DevOps, 자동화, 개발 환경 확장

DevOps와 자동화, 개발자 친화적 환경 구성 역시 다양한 신규 기능이 출시되었습니다. PowerShell, VS Code, CI/CD 연동, Bulk API 등 실무 생산성 향상에 초점이 맞춰진 기능들이 주로 확인되었습니다.

### [PowerShell 모듈로 온프레미스/VNET 데이터 게이트웨이 자동 관리](https://blog.fabric.microsoft.com/en-US/blog/powershell-module-for-gateways-with-expanded-automation-capabilities-generally-available/)
PowerShell 기반 게이트웨이 관리 자동화, 스크립팅을 통한 배포·운영 효율화/보안 자동화 실현.

### [VS Code에서 SQL 데이터베이스 배포 및 Bulk API 지원](https://blog.fabric.microsoft.com/en-US/blog/deploy-sql-databases-in-fabric-from-vs-code-no-more-context-switching/)
VS Code에서 직접 SQL 배포, Bulk Import/Export API로 다량 데이터·워크스페이스 관리 자동화가 실무 환경에 쉽게 적용됩니다.

### [SQL 프로젝트 기반 데이터베이스 DevOps 및 Schema Designer AI 연동(Preview)](https://azure.microsoft.com/updates?id=558155)
Schema-as-code, CI/CD, 코드 품질 체크, AI 기반 스키마 디자인 지원으로 데이터베이스 개발과 DevOps가 통합되었습니다.

### [Databricks Lakeflow Connect – SaaS 무료 tier 및 데이터 유입 확장](https://azure.microsoft.com/updates?id=558810)
Databricks에서 SaaS 데이터 무료 유입, Unity Catalog와의 통합 및 AI/분석 워크로드 가속화.

### [Azure Monitor Log Analytics Summary Rule, Retry bin 기능 도입](https://azure.microsoft.com/updates?id=558656)
요약 규칙 집계 실패시 bin-level 재시도 기능 추가로 데이터 결손 없이 로그 집계 및 분석 자동화 실현.

---

## 총평 및 다음 달 전망

2026년 3월 Azure 업데이트는 '실무 최적화와 AI 실무화의 새로운 표준'을 제시했습니다. Microsoft Foundry와 Fabric이 데이터·AI 기반 실무 환경에 확실한 체계와 관리자동화, 품질평가·관측성, 보안·컴플라이언스를 일원화하며, 단순 PoC를 넘어서 대규모 실운영까지 성장할 수 있는 구조가 강조되었습니다. 인프라와 데이터베이스, 네트워킹·보안의 기초체계 역시 미리보기·신제품·운영관리 기능의 대대적 혁신과 더불어, 장기적 서비스 종료 안내 및 대체 기술 확보가 병행되어 기업의 미래 전략에 실질적 도움을 주는 정책 변화가 지속되었습니다.

다음 달에는 엔터프라이즈 AI 자동화와 데이터 통합, 워크로드 관리, 보안 접근 제어, 멀티클라우드 연동 및 운영 자동화의 추가 혁신이 기대됩니다. 미리보기로 출시된 기능들의 정식 지원(예: AKS 네트워킹, SFTP Entra ID, Storage Mover 등), 데이터플로우 및 파이프라인 관리 개선, 새로운 모델·BI 도구·AI 에이전트 운용 방식의 공식화가 전망됩니다. 전반적으로 “실무에서 검증된 운영관리 체계와 데이터·AI 혁신”이 계속되는 흐름이 유지될 것으로 예측됩니다.
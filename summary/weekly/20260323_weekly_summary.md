# Azure 주간 업데이트 요약 - 2026년 03월 23일

## 🧠 Microsoft Foundry

이번 주 Microsoft Foundry는 엔터프라이즈 현장 적용을 위한 AI 혁신이 두드러집니다. Foundry Agent Service의 정식 지원을 통해 음성 기반 서비스와 엄격한 엔터프라이즈 보안, 네트워크 격리, 모니터링, 인사이트가 실환경에서 제공됩니다. 지속적인 품질 평가·트레이싱 및 옵저버빌리티는 기존 AI 운영의 약점을 보완해주며, 에이전트 개발·운영의 신속성과 안전성이 크게 향상되었습니다. OpenAI GPT-5.4 mini/nano, Nemotron 3 Super 등 첨단 모델의 추가 및 멀티에이전트, 멀티모달, 음성·비정형 데이터 처리까지 확장된 점도 특징입니다. 파트너사 솔루션과의 통합으로 보안 및 거버넌스 요구도 충족하며, Foundry Control Plane을 통한 프레임워크 별 평가/모니터링이 실제 생산 환경에 적용되고 있습니다.

### [정식 지원: 실시간 음성 및 엔터프라이즈 보안을 갖춘 차세대 Foundry Agent Service 출시](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/building-production-ready-secure-observable-ai-agents-with-real/ba-p/4501074)
차세대 Foundry Agent Service가 정식 지원되며, 실시간 음성 접점(Voice Live), 프라이빗 네트워킹, 강화된 트레이싱·보안 및 통합 포털을 제공합니다.

### [NVIDIA Nemotron 3 Super, 오픈/멀티에이전트 최적화 모델 Foundry에서 정식 지원](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/nvidia-nemotron-3-super-now-available-on-microsoft-foundry-open/ba-p/4501781)
NVIDIA Nemotron 3 Super NIM이 Foundry 중심에서 제공되어 대용량, 멀티에이전트 분석 및 맞춤 AI 운영을 Azure 환경에서 지원합니다.

### [OpenAI GPT-5.4 mini 및 nano 모델 정식 출시 및 Foundry 통합](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/introducing-openai-s-gpt-5-4-mini-and-gpt-5-4-nano-for-low/ba-p/4500569)
GPT-5.4 mini/nano가 초저지연·고효율 LLM 환경 제공, 엣지 컴퓨팅 등 다양한 실시간 AI 에이전트 활용에 최적화되어 Foundry에 통합되었습니다.


## 🟦 Microsoft Fabric

Microsoft Fabric 영역에서는 데이터 및 인공지능 플랫폼의 개방성과 자동화, 통합 워크플로우가 확장되었습니다. ISV 및 데이터 엔지니어가 손쉽게 맞춤 워크로드를 게시·운영할 수 있도록 Fabric 확장성과 노트북 퍼블릭 API가 정식 지원됩니다. 데이터 파이프라인 자동화, 예측 기반 플래닝, 실시간 데이터 통합 등 폭넓은 기능이 증대(예: Fabric Data Factory, IQ 플래닝)되어 데이터 기반 경영과 분석, 업무 프로세스 혁신의 토대가 마련되고 있습니다. 파트너사, 오픈소스, 멀티모달 기능이 연계된 생태계 전반의 확장도 주요 변화입니다.

### [정식 지원: Fabric 확장성—셀프서비스 워크로드 게시](https://blog.fabric.microsoft.com/en-US/blog/fabric-extensibility-self-service-workload-publishing-generally-available/)
ISV와 조직별 맞춤 워크로드를 빠르고 손쉽게 게시·유통할 수 있어 Fabric 데이터 생태계 확장 및 자동화가 가속화됩니다.

### [정식 지원: Fabric 노트북 퍼블릭 API](https://blog.fabric.microsoft.com/en-US/blog/fabric-notebook-public-apis-generally-available/)
퍼블릭 API를 통한 노트북 자동화와 워크플로우 통합이 가능해져 데이터 과학·엔지니어의 생산성과 확장성이 높아집니다.

### [정식 지원: Fabric IQ의 예측·플래닝 기능 공개](https://blog.fabric.microsoft.com/en-US/blog/introducing-planning-in-microsoft-fabric-iq-from-historical-data-to-forecasting-the-future/)
Fabric IQ 내 실시간 예측 및 플래닝 지원으로, 과거 데이터 기반 미래경영이 가능해지고 의사결정 자동화가 한층 강화되었습니다.


## 🛡️ 플랫폼·보안·인프라 주요 업데이트

이번 주 Azure 플랫폼·인프라 분야는 하이브리드·멀티클라우드 환경에서 보안, 관리 자동화, 최신 성능 지원이 주목받았습니다. Azure Red Hat OpenShift의 관리형 ID 정식 지원으로 최소 권한 관리를 강화하고, WAF 관리 규칙(DRS 2.2) 정책 업그레이드로 보안 예측력·준수성 향상을 달성하였습니다. Azure SQL Database는 버전리스 키 암호화, 자동지표 유지관리를 도입해 관리 자동화와 보안성을 높였습니다. GitHub Copilot 통합으로 개발 생산성도 향상되고, 대용량 데이터 파이프라인 및 인터페이스 혁신이 이어지고 있습니다.

### [Azure Red Hat OpenShift: 관리형 ID 및 워크로드 ID 정식 지원](https://azure.microsoft.com/updates?id=557917)
OpenShift 클러스터/앱에 AKS와 동일한 최신 ID 정책을 제공, 최소권한 기반 보안 및 Azure 통합 효과 증대.

### [Azure WAF Default Rule Set 2.2 및 규칙 정책 개선](https://azure.microsoft.com/updates?id=558016)
WAF(웹 애플리케이션 방화벽) 최신 규칙 정책으로 N, N-1, N-2 정책 동시 지원과 구버전의 명확한 지원 종료 정책으로 추후 보안 이슈를 사전에 예방할 수 있습니다.

### [Azure SQL Database 투명 데이터 암호화: 버전리스 키로 간소화](https://azure.microsoft.com/updates?id=558183)
버전 없이 최신 키를 자동 사용, 키 관리 자동화 및 운영 리스크 최소화로 데이터 암호화 관리가 단순해집니다.


## 🚨 서비스 지원 종료 및 변경 (Retirement & Deprecation)

다양한 주요 서비스의 지원 종료 일정이 발표되었습니다. HBv2, HC, NP, NVv3, NVv4 등 고성능 VM의 2027년 종료 계획과 Azure Sphere, Windows Server 2016 마켓플레이스 이미지를 포함한 수많은 서비스, 도구들이 차례로 종료 예정입니다. 신규 지원 서비스로의 전환 및 데이터 백업 등 사전 대응이 필수적입니다. Emissions Impact Dashboard도 2027년 3월 종료 예정이니, 대체 솔루션 검토가 권고됩니다.

### [Azure Sphere 2031년 7월 31일 지원 종료](https://azure.microsoft.com/updates?id=557123)
IoT 기기용 Azure Sphere는 2031년 종료. 하드웨어/소프트웨어 대체 및 대안 솔루션 조기 검토 필수.

### [HBv2, HC, NP 시리즈 가상머신 2027년 5월 31일 지원 종료](https://azure.microsoft.com/updates?id=548525)
고성능·AI 연산용 VM 라인업의 단계적 폐기로, HBv5·HX 등 신규 VM군으로 이행 필요.

### [Emissions Impact Dashboard for Azure 지원 종료 예고](https://azure.microsoft.com/updates?id=558278)
2027년 Power BI 기반 탄소 영향 대시보드 서비스 종료. 데이터 이관/백업과 Carbon Optimizer로의 대체 권장.


## ✨ 데이터·AI 통합 및 파트너 연계

데이터 및 AI 파트너십 측면에서는 OneLake, Databricks, Fabric 등 멀티클라우드 환경에서 데이터 자동화와 보안, 멀티모달 AI 접목이 강화되고 있습니다. Azure Databricks와 OneLake의 무복사 데이터 연동(미리 보기)은 데이터 거버넌스와 운영 효율성을 동시에 높여줍니다. 오픈소스 기반의 보안·정책 통합, 써드파티 솔루션 네이티브 연동, 멀티모달·AI 자동화의 전방위 확장으로 데이터 자산 활용폭이 커집니다.

### [Azure Databricks OneLake 카탈로그 연동(미리 보기)로 무복사 데이터 통합](https://azure.microsoft.com/updates?id=558927)
Unity Catalog 연동으로 데이터 복사 없이 OneLake 데이터 자산을 Databricks에서 직접 쿼리할 수 있어 데이터 일관성과 관리 용이성이 증대됩니다.

### [OneLake 보안: 써드파티 솔루션 네이티브 통합](https://blog.fabric.microsoft.com/en-US/blog/third-party-support-for-onelake-security/)
Delta·Iceberg 등 오픈소스 데이터레이크 전반에 걸쳐 일관된 보안정책을 적용, 보안·거버넌스가 단일 프레임워크에서 관리됩니다.

### [Fabric AI 함수의 멀티모달 지원(미리 보기)](https://blog.fabric.microsoft.com/en-US/blog/unlock-insights-from-images-and-pdfs-with-multimodal-support-in-fabric-ai-functions-preview/)
이미지·PDF 등 비정형 데이터에 대한 AI 기반 인사이트 추출이 가능해지며, 데이터/AI 활용 가능성이 확대됩니다.
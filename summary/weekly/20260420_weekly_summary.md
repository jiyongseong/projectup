# Azure 주간 업데이트 요약 - 2026년 04월 20일

## 🗄️ 스토리지 & 관리

지난주 Azure의 스토리지 및 관리 카테고리에서는 하이브리드 스토리지, 클라우드 파일 동기화, 디스크 암호화와 거버넌스, 데이터 티어링 자동화 등 다양한 기능이 정식 지원 또는 신규 출시되었습니다. Smart Tier 자동화 기능은 핫/쿨/콜드 티어간 데이터 이동을 자동화하여 비용을 절감하며, Premium SSD v2와 Ultra Disk의 교차 테넌트 고객관리형 키(CMK) 암호화 지원은 데이터 거버넌스 강화를 위한 유용한 기능입니다. AKS 백업은 단일 CLI 명령으로 손쉽게 설치 및 정책 설정이 가능해 관리 편의성이 높아졌고, Azure File Sync와 Storage Mover는 신규 지역 지원으로 데이터 거버넌스와 레지던시 정책 충족이 강화되었습니다. Azure Files의 프로토콜별 암호화정책, 최소 청구 오브젝트 정책 및 다중 플랫폼 VM 지원 등도 조직의 컴플라이언스, 최적화, 보안 수준을 한층 끌어올렸습니다. 이처럼 Azure는 스토리지의 효율성과 관리 편의, 보안, 지역 확장 등 인프라 전반을 촘촘히 혁신하려는 의지를 이번 업데이트에서 보여줍니다.

### [Smart Tier(Azure Blob 및 Data Lake Storage) 정식 지원 출시](https://azure.microsoft.com/updates?id=559746)
스마트 티어는 핫, 쿨, 콜드 티어 간 자동 이동을 통해 데이터 접근 패턴에 따라 비용을 최적화하는 완전 자동화 솔루션으로, 관리 효율과 비용절감 효과를 제공합니다.

### [Premium SSD v2 및 Ultra Disk 교차 테넌트 CMK 암호화 정식 지원](https://azure.microsoft.com/updates?id=559761)
타 Microsoft Entra 테넌트의 고객관리형 키를 이용해 디스크 암호화가 가능해져, 데이터 거버넌스와 다중 테넌트 환경에서 보안 유연성이 강화되었습니다.

### [AKS 백업 구성 단일 CLI 명령 지원](https://azure.microsoft.com/updates?id=560521)
AKS 백업 설정이 단 한 줄의 CLI 명령으로 자동화되어, 설치부터 정책설정까지 모든 백업 관리가 더욱 간편하게 이루어집니다.

---

## ⚡ 컴퓨팅 및 네트워크

컴퓨팅 및 네트워크 영역에서는 AKS의 네트워크 확장성과 운영 체제 지원, VM 시리즈 지원 종료 등이 주요 이슈였습니다. AKS 클러스터는 StandardV2 NAT Gateway outbound 타입 출시로 zone-redundant, 최대 100Gbps, IPv6 네트워크 지원을 받아 대규모 애플리케이션의 안정적 운영이 가능해졌습니다. Ubuntu 22.04 OS의 AKS 지원 종료 예정은 기업의 마이그레이션 및 OS 업그레이드 필요성을 강조하며, 장기적 보안 및 성능 관점에서 권장조치가 강조됩니다. 또한 Batch Pool에서 HBv2/HC/NP VM 시리즈의 지원 종료가 2027년 예정되어, 새로운 VM 시리즈 및 GPU 기반으로의 마이그레이션 계획이 필요합니다. 전반적으로 인프라 플랫폼의 지속적 진화와 최신 표준 준수가, 대규모 클라우드 워크로드에 필요한 핵심 환경을 구축하는 흐름을 나타냅니다.

### [AKS StandardV2 NAT Gateway outbound 타입 지원](https://azure.microsoft.com/updates?id=560207)
최대 100Gbps의 outbound 네트워크와 IPv6 지원을 통해 AKS 클러스터의 네트워크 확장성과 안정성이 크게 강화되어 대규모 애플리케이션 운영에 최적화됩니다.

### [AKS에서 Ubuntu 22.04 지원 종료 예정](https://azure.microsoft.com/updates?id=557928)
2027년 6월 30일부터 AKS에서 Ubuntu 22.04 지원이 종료될 예정이며, 모든 사용자는 Ubuntu 24.04(이후)로 마이그레이션을 권장받습니다.

### [Azure Batch Pool VM(HBv2, HC, NP) 시리즈 지원 종료](https://azure.microsoft.com/updates?id=559751)
2027년 5월 31일부로 HBv2, HC, NP 시리즈 VM들이 Batch Pool에서 지원이 종료되며, 최신 VM 시리즈로의 마이그레이션이 요구됩니다.

---

## 💡 인공지능(AI) & 분석

AI 및 분석 분야에서는 Azure Databricks에서 Claude Opus 4.7 모델 정식 지원, AutoML 기반 이미지 분류 자동화, LLM 추론을 위한 병렬처리 기반 인퍼런스 최적화 등의 혁신이 돋보였습니다. Azure Databricks의 최신 AI 모델은 고급 문서 분석과 에이전트 구축에 최적화되어, 복잡한 기업 워크로드에 높은 정확도와 효율성을 제공합니다. Azure Machine Learning의 AutoML은 이미지 분류, 결함 감지 등의 현장 적용 시나리오에서 데이터 전처리, 하이퍼파라미터 튜닝, 에지 배포까지 완전 자동화 프로세스를 구현해 개발과 운영 효율성을 극대화합니다. 또한 Azure OpenAI의 병렬 처리 기반 추론 파이프라인은 LLM 처리 속도를 20배 이상 높이며, 대량 데이터셋 인퍼런스 및 API Rate Management를 통해 생산성 향상과 비용 효율을 동시에 달성할 수 있습니다. 현장 중심의 대규모 비정형 데이터 활용, 클라우드-엣지 연동, 운영 자동화 등 AI의 실용적 전환이 급진전되고 있습니다.

### [Azure Databricks에서 Claude Opus 4.7 정식 지원](https://azure.microsoft.com/updates?id=560590)
Anthropic의 최신 LLM인 Claude Opus 4.7이 Databricks에서 제공되어, 기업 AI 혁신에 필요한 고급 문서 분석과 에이전트 구축이 손쉽게 지원됩니다.

### [Azure AutoML 이미지 분류 자동화 활용 사례](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/simplifying-image-classification-with-azure-automl-for-images-a/ba-p/4479632)
Azure Machine Learning의 AutoML로 이미지 분류 및 결함 감지 등 복잡한 현장 분석을 완전 자동화하여 클라우드-엣지 연동을 지원합니다.

### [Azure OpenAI 병렬 처리로 LLM 추론 성능 최적화](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/friends-don-t-let-friends-run-loops-sequentially/ba-p/4505815)
병렬 처리 파이프라인을 활용해 LLM 인퍼런스 속도를 최대 20배 이상 향상시키며, 대량 AI 활용 효율과 비용 관리 사례를 실질적으로 제시했습니다.

---

## 🔥 Microsoft Foundry

Microsoft Foundry에서는 AI 모델 파인튜닝, 비용 효율화, 멀티모달 헬스케어 AI, 혁신적 모델 통합, MCP 연동 등 AI 모델 R&D 및 엔터프라이즈 혁신에 초점을 맞춘 대형 업데이트가 이어졌습니다. o4-mini 글로벌 파인튜닝 가격 인하, GPT-4.1 평가자 도입, 강화학습 기반 Reinforcement Fine-Tuning 안내서 제공 등은 기업의 AI R&D 프로세스와 특화 모델 생산성을 획기적으로 개선합니다. Microsoft Harrier와 NVIDIA EGM-8B 등 최신 임베딩 및 비전-언어 모델 통합은 다양한 AI 워크플로우를 확장하며, GigaTIME 멀티모달 헬스케어 AI, OneLake MCP 연동은 대규모 의료데이터와 R&D, 연구자 진단 혁신에 직접적으로 기여합니다. 또한 MAI-Image-2-Efficient, Copilot 등 실무 및 현장 적용형 AI 서비스의 확대는 Foundry 기반 AI 개발·운영의 혁신적 변화와 현장 효율화를 실증합니다.

### [Microsoft Foundry 파인튜닝 최신 업데이트(2026년 4월)](https://devblogs.microsoft.com/foundry/whats-new-in-foundry-finetune-april-2026/)
o4-mini 글로벌 파인튜닝 가격 인하, GPT-4.1 평가자 도입, Reinforcement Fine-Tuning 가이드 공개 등 AI 모델 훈련 및 관리가 더욱 효율적으로 변화했습니다.

### [Microsoft Harrier & NVIDIA EGM-8B Foundry 통합](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/now-in-foundry-microsoft-harrier-and-nvidia-egm-8b/ba-p/4510851)
최신 멀티언어 임베딩 모델과 비전-언어 모델이 Foundry에 통합되어, 고성능 AI 활용 및 모델 선택 폭이 확대되었습니다.

### [GigaTIME 멀티모달 헬스케어 AI Foundry 지원](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/bringing-gigatime-to-microsoft-foundry-unlocking-tumor/ba-p/4509452)
의료 데이터 공간 분석·암 미세환경 연구를 위한 GigaTIME 모델이 Foundry 플랫폼에 도입되어 생명과학 연구 혁신을 실현합니다.

---

## 🚀 Microsoft Fabric

이번주 Microsoft Fabric에서는 OneLake 카탈로그 탐색 및 관리자 거버넌스 정식 지원, 데이터 클러스터링, 병렬 파티션 처리, 민감도 레이블 API, SSMS Warehouse 관련 기능, Workspace 태깅 등 대규모 데이터 거버넌스와 관리, 성능 혁신을 위한 업데이트가 다수 이루어졌습니다. OneLake 카탈로그는 Copilot·Excel 연동, 테이블·컬럼 검색, 부모-자식 구조화, 도메인별 관리 등으로 사용자 경험을 혁신하며, 병렬 파티션 컴퓨트 정식 지원 예정은 대용량 데이터 처리 성능을 획기적으로 향상시킵니다. 데이터 클러스터링, 외부 데이터 소스 지원, 다이내믹 태깅, 민감도 레이블 API 등은 Fabric 내 거버넌스·컴플라이언스 확보, Workspace 관리 효율화를 동시에 실현합니다. 마지막으로 SSMS의 Fabric Warehouse 전용 기능은 DB 관리자들의 생산성을 대폭 높였습니다. 이번 Fabric 로드맵은 데이터 중심 조직의 클라우드 거버넌스와 확장성을 한 층 끌어올리는 결과를 보여줍니다.

### [OneLake 카탈로그 탐색 기능 정식 지원](https://www.fabric-gps.com/release/86a39e25-2f62-f011-bec2-000d3a302e4a)
OneLake 카탈로그의 탐색·거버넌스 기능이 강화되어 Copilot, Excel 연동, 부모-자식 구조, 도메인별 아이템 관리 등 데이터 관리 경험이 대폭 향상되었습니다.

### [Dataflows Gen2 파티션 병렬처리 정식 지원 예정](https://www.fabric-gps.com/release/385260b0-5b07-ef11-9f89-000d3a34b75c)
병렬 파티션 컴퓨트로 대용량 데이터 변환·처리 성능을 획기적으로 개선하며, Fabric 내 안정적·확장가능한 데이터 처리 기반이 마련됩니다.

### [OneLake 카탈로그 관리자 거버넌스 기능 정식 지원](https://www.fabric-gps.com/release/a328d155-cf01-f111-8406-6045bd0a8ec1)
Fabric 관리자용 Govern 기능이 정식 지원되어 도메인, 용량, 워크스페이스, 보호 상태, 권장 작업 등 조직 전체 데이터 거버넌스 강화가 가능합니다.
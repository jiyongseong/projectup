# Azure 주간 업데이트 요약 - 2026년 04월 06일

## 🧠 Microsoft Foundry 및 AI 서비스 요약
지난주 Microsoft Foundry와 Azure AI 서비스에서는 엔터프라이즈 AI 플랫폼 강화와 AI 모델 관리 모범 사례가 집중적으로 다루어졌습니다. NVIDIA, IBM, Sarvam 등 초대형 AI 모델이 Foundry를 통해 Hugging Face 컬렉션에 추가되어 초장문·다국어·음성 처리가 더욱 개선되었습니다. MAI 음성 및 이미지 생성 AI 모델(미리 보기)이 도입되어 실시간 대화, 고품질 멀티미디어 활용, Azure Speech API 연동까지 엔터프라이즈급 성능 확장을 지원합니다. 모델 업그레이드·마이그레이션 전략이 공개되어 책임 있는 AI 운영, 중앙화된 모델 인벤토리, 오프라인/온라인 평가 프로세스가 일상적으로 정착되고 있습니다. 또한 지속 메모리, Voice Native Agent, TSGen 사례 등 사용자 맞춤형 AI 기능과 실무 자동화 솔루션이 선보여 기업 신뢰성과 확장성이 한층 강화된 한 주였습니다.

### [Foundry의 새로운 AI 모델: NVIDIA Nemotron-3-Super-120B, IBM Granite-4.0 및 Sarvam-105B 지원](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/now-in-foundry-nvidia-nemotron-3-super-120b-a12b-ibm-granite-4-0/ba-p/4506917)
최신 초대형 AI 모델이 Foundry에서 Hugging Face 컬렉션을 통해 도입되어 초장문, 음성, 다국어, 특화 워크로드에 바로 활용할 수 있습니다.

### [MAI 음성·이미지 AI모델(미리 보기) 출시](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/introducing-mai-transcribe-1-mai-voice-1-and-mai-image-2-in/ba-p/4507787)
실시간 음성인식, 텍스트-음성, 텍스트-이미지 생성 모델이 Foundry에 공개되어 멀티미디어 AI 활용성과 Azure Speech API 연동이 대폭 강화되었습니다.

### [Foundry 모델 업그레이드와 마이그레이션 전략](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/model-upgrade-and-migration-strategy-for-microsoft-foundry/ba-p/4503176)
모델 버전 중앙화 관리, 운영 리스크 최소화, 평가 체계 정립 등 책임 있는 AI 모델 운영 정책과 실무 적용 방법이 상세히 제시되었습니다.

---

## 📈 Microsoft Fabric 주요 업데이트 요약
Microsoft Fabric에서는 자동화·보안·데이터 거버넌스와 사용자 경험 개선이 집중적으로 이루어졌습니다. OneLake 파일 탐색기가 정식 지원되어 데이터 조직 및 생산성이 크게 향상되었고, ML 실험/모델/Spark에 대한 아웃바운드 접근 보호가 도입되어 엔터프라이즈 데이터 보안이 한층 강화되었습니다. Databricks Private Link 연동, Translytical 태스크 플로우, 공공API 민감도 라벨 관리 등 데이터 레이크와 분석 환경의 기능 확장이 활발하게 진행되었으며, 시각화 테마, 테이블 커스텀 합계 등 보고서 현대화 기능도 함께 제공됐습니다. BYOK 암호화, Ontology Private Link 미리 보기 등 보안 기술이 진화했고, SQL DB 자동스케일, MDM 연동 등 확장성과 비용 효율성 개선도 두드러진 한 주였습니다.

### [OneLake 파일 탐색기 정식 지원](https://www.fabric-gps.com/release/c265c7b8-09b9-f011-bbd3-6045bd00f9db)
OneLake에 파일 탐색기 기능이 정식 지원되어 데이터 관리와 생산성이 크게 향상되었습니다.

### [ML 실험·Spark에 아웃바운드 접근 보호 기능 도입](https://www.fabric-gps.com/release/635cb2b6-6324-f011-8c4d-000d3a34671f)
외부 데이터 유출 차단과 선택적 연결 허용이 가능해져 엔터프라이즈 보안 기반의 ML 및 Spark 환경 신뢰성이 높아졌습니다.

### [Fabric 공공API 민감도 라벨 관리 정식 지원](https://blog.fabric.microsoft.com/en-US/blog/sensitivity-labels-in-fabric-for-public-apis-generally-available/)
Microsoft Purview 기반 민감도 라벨이 API 관리로 확장되어 정보 분류, 자동화 워크플로우, AI 연동이 쉬워졌습니다.

---

## 💾 스토리지 및 인프라 서비스 주요 업데이트
스토리지 및 인프라 부문에서는 Azure NetApp Files의 cool access 기능 강화와 Data Box 자동 Secure Erasure 인증서, Azure Files Provisioned v2 지원 등 데이터 보안과 유연성이 크게 개선되었습니다. 이벤트 아키텍처 최적화를 위한 Event Grid MQTT 메시지 정렬, 연결 제한, 세분화 등도 출시됐으며, 태블/큐/파일의 User Delegation SAS로 데이터 보안이 한층 강화되었습니다. Azure Red Hat OpenShift 인도네시아 정식 지원, 덴마크 신규 리전 오픈, 프리미엄 SSD v2의 글로벌 리전 확장 등 글로벌 인프라 접근성이 상승하였고, 클라이언트 측 구성 대규모 안전 제공, Ephemeral OS 디스크 완전 캐싱 미리 보기로 VM/VMSS 속도와 신뢰성도 향상되었습니다.

### [Azure NetApp Files: cool access 기능 강화(미리 보기)](https://azure.microsoft.com/updates?id=559504)
핫/쿨 워크로드에 적합한 자동 튜닝 cool access 기능이 추가되어 성능과 비용 효율성 및 사용 경험이 크게 개선되었습니다.

### [Azure Data Box: 자동 Secure Erasure 인증서 지원](https://azure.microsoft.com/updates?id=559772)
NIST 기준에 부합하는 데이터 삭제 인증서가 자동 생성·다운로드되어 규제 및 감사 대응이 간편해졌습니다.

### [Azure Tables/Files/Queues에서 User Delegation SAS 정식 지원](https://azure.microsoft.com/updates?id=559535)
사용자가 위임 방식으로 SAS 토큰을 생성·관리할 수 있게 되어 보안과 접근 제어의 세분화가 동시 실현되었습니다.

---

## 🛠️ 서비스/기능 지원 종료 & 정책 변화
서비스 및 기능의 지원 종료 관련 안내에서는 Cosmos DB for PostgreSQL, AzureDnsEndpoints, Prometheus sidecar, ML 외부 데이터 연결, Python App Service/Functions on Windows, Azure AI Language 주요 기능, 서비스 패브릭의 Windows Server 2019/2022 등 다양한 영역의 사용 중단 일정과 대체 방안이 제공되었습니다. Elastic Cluster 마이그레이션, Standard 엔드포인트 전환, 직접 remote-write 구성 등 엔터프라이즈 운영자의 사전 대응을 위한 정책과 마이그레이션 절차가 강조되고 있습니다. 모델 업그레이드, 버전 관리 정책 및 Responsible AI 운영이 제도화되어 서비스 중단 리스크 대응이 용이해졌습니다.

### [Azure Cosmos DB for PostgreSQL 지원 종료(2029년 3월 31일)](https://azure.microsoft.com/updates?id=556085)
Elastic Cluster로 데이터 마이그레이션이 필요하며, 기능 및 가격 혜택과 향후 서비스 안정성을 위해 사전 전환이 권장됩니다.

### [Python App Service/Functions on Windows 사용 중단(2027년 3월 31일)](https://azure.microsoft.com/updates?id=558027)
Python 워크로드는 Azure Linux 플랫폼으로 이전이 필요하며, 기존 구성 및 데이터는 유지되나 앱 실행이 불가합니다.

### [Azure AI Language 주요 8개 기능 사용 중단(2027년 3월 20일)](https://azure.microsoft.com/updates?id=557394)
키워드 추출, 감정 분석 등 주요 기능이 중단되며, Microsoft Foundry 기반 대체 및 이전 전략이 권장됩니다.

---

## 🌏 글로벌 및 지역(한국 포함) 서비스 업데이트
글로벌 Azure 확장과 지역별 안정성 강화를 위한 업데이트가 추진되었습니다. 덴마크 신규 리전 개설로 현지 고객의 데이터 거주, 저지연, 고급 클라우드·AI 서비스 이용이 가능하게 되었습니다. 프리미엄 SSD v2 디스크가 인도·미국 정부 리전으로 확장되어 엔터프라이즈 대용량 IO 워크로드에 효율적 처리 지원이 강화되었습니다. Azure Red Hat OpenShift 인도네시아 정식 지원으로 현지 규제 대응, 현대화 및 하이브리드 클라우드 운영 환경이 넓어졌습니다. 한국(코리아 중앙, 코리아 남부) 내 신규 업데이트 항목은 이번 주에는 포함되어 있지 않습니다.

### [Microsoft Azure 덴마크 신규 클라우드 리전 출시](https://azure.microsoft.com/updates?id=559406)
현지 고객의 데이터 거주, 낮은 지연, AI 플랫폼 서비스 활용 등 현지화 전략이 뚜렷하게 강화되었습니다.

### [Azure Premium SSD v2 디스크 인도 및 US Gov Arizona 리전 지원](https://azure.microsoft.com/updates?id=559526)
다양한 엔터프라이즈 워크로드에 고성능·저비용 저장 옵션이 확대되어, 미사용 리전에서도 지원 요청이 가능합니다.

### [Azure Red Hat OpenShift 인도네시아 중앙 리전 정식 지원](https://azure.microsoft.com/updates?id=559552)
현지 규제·데이터 거주, 네트워크·보안 통합 등 하이브리드 클라우드 운영과 앱 현대화가 보다 쉽게 실현됩니다.
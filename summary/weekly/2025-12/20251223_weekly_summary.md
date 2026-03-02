# Azure 주간 업데이트 요약 - 2025-12-23

## 📦 스토리지
지난주 Azure 업데이트에서는 스토리지 분야에서 중요한 내용들이 발표되었습니다. 랜섬웨어 방지 기능과 데이터 복제 기능이 주목받았습니다. 특히, Azure NetApp Files의 고급 랜섬웨어 방지 기능은 이제 미리 보기 상태로 제공되며 클라우드 환경에서 랜섬웨어를 효과적으로 분석하고 대응할 수 있는 기능을 포함합니다. 이와 함께 AZ-존 간 복제를 통해 데이터 볼륨 복제 기능이 정식 지원 상태로 발표되었습니다. 또한 Azure Blob 간 데이터를 간편하게 이동할 수 있는 기능이 소개되어 사용자의 데이터 작업을 더욱 쉽게 만들어줍니다.

### [Azure NetApp Files 고급 랜섬웨어 방지 기능 - 미리 보기](https://azure.microsoft.com/updates?id=536699)
Azure NetApp Files의 랜섬웨어 방지 기능은 파일 확장자와 IOPS 패턴을 통해 데이터 볼륨에 대한 위협을 초기에 탐지하고 자동으로 대응합니다.

### [Azure NetApp Files 교차-존-지역 복제 - 정식 지원](https://azure.microsoft.com/updates?id=537106)
지역 및 가용성 존 간 데이터 볼륨을 복제하여 재해 복구와 비즈니스 연속성을 더욱 강화합니다.

### [Azure Blob-to-Blob 간편 이동 - 미리 보기](https://aka.ms/learnblobtoblob)
Azure Storage Mover를 활용해 Blob 컨테이너 간 데이터를 더 간편하고 빠르게 이동할 수 있습니다.

---

## 🗄️ 데이터베이스
데이터베이스 분야에서는 성능과 운영 효율성을 개선하기 위한 도구들이 소개되었습니다. Azure Cosmos DB의 새로운 SRE 에이전트는 데이터베이스 워크로드 상태를 더 깊게 분석하여 문제가 발생한 영역을 신속하게 식별할 수 있도록 도와줍니다. 또한 Azure SQL 데이터베이스에서는 서버리스 작업을 최적화하고 자동 재개 원인을 분석할 수 있는 활동 로그 기능이 정식으로 도입되었습니다.

### [Azure Cosmos DB SRE 에이전트 활용 - 미리 보기](https://azure.microsoft.com/updates?id=541813)
Azure Cosmos DB의 SRE 에이전트를 통해 데이터 워크로드 성능을 분석하고 문제에 대한 자동화된 해결책을 제시받을 수 있습니다.

### [Azure SQL 업데이트 - 정식 지원](https://azure.microsoft.com/updates?id=541818)
서버리스 작업의 자동 재개 원인을 분석하여 데이터 액세스 패턴을 최적화할 수 있는 기능이 추가되었습니다.

---

## 🖥️ 컴퓨트
컴퓨트 카테고리에서는 Azure Functions의 SDK 타입 바인딩 기능이 확장되었습니다. 특히 JavaScript와 TypeScript를 이용한 애플리케이션에서 Azure Blob Storage 및 Service Bus와 상호작용할 수 있는 기능이 도입되었습니다. 이를 통해 개발자가 더 쉽게 고급 메시징 기능을 활용할 수 있도록 돕습니다.

### [Azure Functions Service Bus SDK 타입 바인딩 - 미리 보기](https://azure.microsoft.com/updates?id=541427)
JavaScript 및 TypeScript에서 Service Bus와 상호작용할 수 있는 타입 바인딩 지원 기능이 도입되어 개발 편의성이 크게 향상됩니다.

---

## 🌐 하이브리드 및 멀티 클라우드
하이브리드 및 멀티 클라우드에서는 클라우드 아키텍처 전반에서 성능 최적화를 위한 다양한 향상된 기능이 발표되었습니다. 특히 Azure SQL의 새로운 기능은 서버리스 워크로드의 자동 복구 원인을 파악하고 최적화하는 데 유용합니다. 이는 운영 효율성을 강화하는 데 중요한 역할을 합니다.

### [Azure SQL 서버리스 워크로드 분석 - 정식 지원](https://azure.microsoft.com/updates?id=541818)
서버리스 작업의 성능을 높이고 자동 복구 과정을 분석하여 데이터베이스 운영을 최적화합니다.

---

## 🚀 마이그레이션
마이그레이션 업데이트에서는 데이터 이동을 간소화하기 위한 새로운 기능이 제공되었습니다. Azure Storage Mover의 블롭 간 데이터 이전 기능은 작업의 복잡성을 줄이고 대규모 데이터 이동을 자동화하여 운영 효율성을 크게 향상합니다.

### [Azure Storage Mover 블롭 간 데이터 이동 - 미리 보기](https://azure.microsoft.com/updates?id=542813)
자동화와 실시간 가시성을 제공하며, 대규모 데이터 이동을 안전하고 효과적으로 처리할 수 있는 Blob-to-Blob 이전 기능이 미리 보기 상태로 출시되었습니다.
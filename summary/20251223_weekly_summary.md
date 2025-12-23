# Azure 주간 업데이트 요약 - 2023년 10월 18일

Azure의 최신 업데이트 내용을 카테고리별로 정리하고 요약하였습니다. 이번 주에는 스토리지, 컴퓨팅, 데이터베이스, 클라우드 운영 및 마이그레이션, 그리고 컨테이너 및 IoT 영역에서 주목할 만한 많은 기능이 추가되고 개선되었습니다.

---

## 🗂 스토리지

Azure의 스토리지 관련 주요 업데이트는 데이터 보안과 복구에 초점이 맞추어져 있습니다. 특히 Azure NetApp Files를 활용한 랜섬웨어 보호 기능의 추가와 교차 영역-지역 복제 기능의 정식 지원은 사용자 데이터의 보안과 재해 복구 능력을 강화합니다. 또한 Azure Storage Mover를 통해 Blob 간 데이터를 손쉽게 이동할 수 있어 클라우드 간 데이터 이전 솔루션이 더욱 간편하고 효율적으로 제공됩니다. 이러한 업데이트는 데이터 저장소가 보다 안전하고 유연하게 기능하도록 지원합니다.

### [Azure NetApp Files 고급 랜섬웨어 보호 [미리 보기]](https://azure.microsoft.com/updates?id=536699)
Azure NetApp Files에 랜섬웨어 탐지와 데이터를 보호하는 기능이 추가되었습니다. 의심스러운 활동이 감지되면 즉시 스냅샷을 생성하여 복구를 신속히 수행할 수 있습니다.

### [Azure NetApp Files 교차 영역-지역 복제 [정식 지원]](https://azure.microsoft.com/updates?id=537106)
이제 Azure NetApp Files에서 데이터 복제를 교차 영역 또는 지역 간에서도 수행할 수 있습니다. 이는 재해 복구와 데이터 가용성의 강화를 위한 핵심 기능으로 제공됩니다.

### [Azure Blob-to-Blob 이전 간소화 [미리 보기]](https://azure.microsoft.com/updates?id=542813)
Blob 컨테이너 간 데이터 이전을 더 단순하고 빠르게 수행할 수 있도록 하는 기능이 추가되었습니다. 대량 데이터의 클라우드 이동을 지원합니다.

---

## 🚀 컴퓨팅

Azure Functions에서 Node.js 기반의 Service Bus SDK 타입 바인딩 기능을 지원하기 시작했습니다. 이를 통해 개발자들은 고급 메시징 기능을 활용하며, JavaScript 및 TypeScript 애플리케이션에서 ServiceBusMessageContext 타입을 사용하여 더욱 간편하게 서비스와 데이터를 통합할 수 있습니다. 컴퓨팅 영역의 새로운 기능은 프로세스를 간소화하고 클라우드 네이티브 애플리케이션 개발을 더욱 손쉽게 만듭니다.

### [Azure Functions의 Service Bus SDK 타입 바인딩 [미리 보기]](https://azure.microsoft.com/updates?id=541427)
Node.js 환경에서 Azure Functions가 Service Bus SDK 타입 바인딩을 지원하여 강력한 서비스 통합을 제공합니다.

---

## 📚 데이터베이스

데이터베이스 업데이트는 Azure SQL과 Cosmos DB에서 중요한 기능 개선이 이루어졌습니다. Azure SQL의 활동 로그는 서버 없는 작업의 고급 최적화를 가능하게 하고, Azure Cosmos DB는 SRE 에이전트를 통해 상태와 성능 모니터링을 간소화했습니다. 이는 데이터 애플리케이션 개발자들에게 중요한 정보를 제공하고 작업 효율을 크게 향상시킵니다.

### [Azure SQL 업데이트 [정식 지원]](https://azure.microsoft.com/updates?id=541818)
Azure SQL에서 서버 없는 워크로드의 활동 로그를 통해 작업 재개 패턴을 최적화할 수 있습니다.

### [Azure Cosmos DB SRE 에이전트 [미리 보기]](https://azure.microsoft.com/updates?id=541813)
Azure Cosmos DB의 SRE 에이전트는 클라이언트와 서버 측 테이블 데이터의 통합 진단을 지원하여 성능 모니터링을 간소화합니다.

---

## 🌐 클라우드 운영 및 마이그레이션

Azure Storage Mover가 개선되어 Blob-to-Blob 데이터 이전이 더 간편하고 빠르게 이루어집니다. 이 기능은 대량 데이터를 전송해야 하는 환경에서 시간 소요를 줄이고 업무 프로세스를 간소화하는 데 큰 도움을 줍니다.

### [Azure Storage Mover [미리 보기]](https://azure.microsoft.com/updates?id=542813)
Blob 컨테이너 간 대량 데이터 이전을 안전하고 신속하게 진행할 수 있는 자동화 서비스가 추가되었습니다.

---

## ⬢ 컨테이너와 IoT 

컨테이너 환경에서 Service Bus SDK 타입 바인딩을 지원하여 더욱 강력한 통합 기능이 제공되었으며, IoT 영역에서도 Cosmos DB와의 결합을 통해 고급 모니터링과 데이터 관리 기능이 강화되었습니다.

### [Azure Functions 지원 향상 [미리 보기]](https://azure.microsoft.com/updates?id=541427)
Service Bus SDK 타입 바인딩을 제공하여 컨테이너 기반 애플리케이션 개발을 더욱 효율적으로 지원합니다.

### [Azure Cosmos DB와 SRE 에이전트 [미리 보기]](https://azure.microsoft.com/updates?id=541813)
IoT 애플리케이션에서 Cosmos DB와 SRE 에이전트를 연결하여 더 높은 수준의 데이터 가시성과 안정성을 확보할 수 있습니다.

--- 

이번 주에 발표된 Azure의 업데이트는 다양한 사용 사례와 유스 케이스에 걸쳐 클라우드 작업의 효율성과 보안을 강화하는 방향으로 이루어졌습니다.
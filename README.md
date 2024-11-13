# 3fy


# 3fy Project

1. 관리 서비스: optify
    - 사용자가 필요한 옵션을 선택하고 설정을 관리하는 역학을 담당합니다.
    - 이 서비스는 사용자로부터 필요한 기능이나 컴포넌트를 선택받아 해당 설정을 저장합니다. 저장된 설정은 사용자 웹 서비스에서 사용될수 있도록 API나 데이터베이스에 저장 할수 있습니다.
    
2. 사용자 웹 서비스: nacfy
    - 사용자가 관리 서비스에서 선택한 옵션에 따라 필요한 기능만을 사용할 수 있는 웹서비스 입니다.
    - 이 서비스는 관리 서비스의 설정을 참조하여, 조건부로 필요한 컴포넌트만 로딩하여 사용자에게 보여줍니다.  Rest API나  GraphQL을 통해서 설정을 불러와서 컴포넌트를 동적으로 임포트하고 렌더링 할 수 있습니다.
3. 기능 제공 웹 서비스: scriptfy
    - 컴포넌트와 기능을 사용자 웹서비스에 제공하는 역학을 담당합니다.
    - 이 서비스는 공통 기능과 컴포넌트를  API로 제하거나 모듈로 공유하여 사용자 웹서비스가 필요한 경우 해당 컴포넌트를 요청하고 사용할 수 있게 합니다.
    - 독립된 서비스로 유지해 다양한 기능을 확장하기 쉽게 만들고, 필요한 경우 웹 서비스에서만 로드 되도록 설정할수 있습니다.


# 3fy Project
1. Management Service: optify
    - This service handles the role of allowing users to select and manage the settings they need.
    - It collects and stores the required functionalities or components chosen by the user. The saved configurations can be stored in an API or database so that they can be used by the user web service.
2. User Web Service: nacfy
    - This is a web service that allows users to access only the functionalities they need, based on the options selected in the management service.
    - This service references the settings from the management service and conditionally loads and displays only the required components to the user. It can dynamically import and render components using settings fetched via REST API or GraphQL.
3. Function Provision Web Service: scriptfy
    - This service is responsible for providing components and functionalities to the user web service.
    - It delivers shared functionalities and components through APIs or modules so that the user web service can request and utilize the needed components when necessary.
    - By maintaining it as a standalone service, it makes it easier to expand various functionalities and ensures that components are only loaded when needed by the web service.

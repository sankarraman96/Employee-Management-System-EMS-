# Employee-Management-System-EMS

Project: Employee Management System (EMS)Project OverviewEmployee Management System (EMS) is an enterprise web application developed to streamline HR operations and employee lifecycle management. The system enables organizations to manage employee information, attendance, leave requests, payroll processing, document management, and reporting through a centralized platform.The application supports role-based access for HR Administrators, Managers, and Employees. It was designed using a modern Angular frontend and .NET 9 backend architecture with secure authentication, Azure cloud integration, and microservices-ready design principles.The system also integrates Azure Blob Storage for secure document storage and RabbitMQ for asynchronous communication between services such as Leave Management and Payroll.

Technology StackFrontend TechnologiesAngular 19TypeScriptBootstrap 5SCSSRxJSAngular Reactive Formsng-Bootstrapag-Gridng2-ChartsJasmineKarma

Backend Technologies.NET 9 / ASP.NET Core 9Web APIsMinimal APIsDapperEntity Framework Core (legacy modules)FluentValidationAutoMapperNUnitNSubstituteFluent Assertions

SecurityJWT AuthenticationOAuth2OpenID ConnectRole-Based AuthorizationPolicy-Based Authorization

DatabaseSQL Server 2022Stored ProceduresViewsDatabase ScriptsDatabase Versioning

Cloud & StorageAzure Blob StorageAzure App ServiceAzure Key VaultAzure Application Insights

Messaging & IntegrationRabbitMQREST APIsSOAP/WCF Integration (legacy payroll service)

DevOps & DeploymentGitHubGitHub ActionsGitHub CodeQLDependabotIISDockerCI/CD Pipeline

ArchitectureAngular 19 Application
         |
     API Gateway
         |
------------------------------------------------
|              |              |                |
Employee     Leave         Payroll         Auth
Service      Service       Service         Service
     |            |            |
     |         RabbitMQ        |
     |_________________________|
                |
           SQL Server
                |
        Azure Blob Storage


Business ModulesEmployee ManagementAdd EmployeeUpdate Employee DetailsEmployee SearchEmployee TransferEmployee Status ManagementEmployee Profile Management

Department ManagementDepartment CreationEmployee AssignmentDepartment Reporting

Leave ManagementApply LeaveLeave Approval WorkflowLeave Balance CalculationLeave History Tracking

Attendance ManagementDaily AttendanceCheck-InCheck-OutAttendance Reports

Payroll ManagementSalary ProcessingLeave DeductionsPayroll ReportsPayslip Generation

Document ManagementDocuments stored in Azure Blob Storage:
Employee Profile PhotosResumesOffer LettersExperience CertificatesPayslipsLeave Attachments

Dashboard & AnalyticsManagement Dashboard includes:
Employee Count by DepartmentMonthly Attendance StatisticsLeave TrendsPayroll SummaryNew Joiners Report
Implemented using:
ng2-Chartsag-Grid

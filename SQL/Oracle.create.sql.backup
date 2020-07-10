



CREATE TABLE "Employee"
(

	"primaryKey" RAW(16) NOT NULL,

	"Surname" NVARCHAR2(255) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	"Patronymic" NVARCHAR2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "EquipmentModel"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	"Manufacturer" RAW(16) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "TypeOfEquipment"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "MaintenancePlan"
(

	"primaryKey" RAW(16) NOT NULL,

	"StartDate" DATE NULL,

	"EndDate" DATE NULL,

	"Equipment" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "PurposeOfTheMaintenanceModel"
(

	"primaryKey" RAW(16) NOT NULL,

	"EquipmentModel" RAW(16) NOT NULL,

	"MaintenanceProgram" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "FactOperationOfTheMaintenance"
(

	"primaryKey" RAW(16) NOT NULL,

	"ExecutionDate" DATE NOT NULL,

	"Successfully" NUMBER(1) NOT NULL,

	"ScheduledMaintenanceOperation" RAW(16) NULL,

	"MaintenanceOperation" RAW(16) NOT NULL,

	"FactOfTheMaintenance" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "FactOfTheMaintenance"
(

	"primaryKey" RAW(16) NOT NULL,

	"StartDate" DATE NULL,

	"EndDate" DATE NULL,

	"ScanProtocol" NVARCHAR2(255) NULL,

	"MaintenancePlan" RAW(16) NULL,

	"Equipment" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "Equipment"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NULL,

	"ProductionDate" DATE NULL,

	"DateOfCommissioning" DATE NULL,

	"WarrantyPeriod" DATE NULL,

	"OperatingTime" NUMBER(10) NULL,

	"RunDate" DATE NULL,

	"Description" NVARCHAR2(255) NULL,

	"Accountable" RAW(16) NOT NULL,

	"SupplyContract" RAW(16) NULL,

	"Model" RAW(16) NOT NULL,

	"Location" RAW(16) NOT NULL,

	"Status" RAW(16) NOT NULL,

	"Type" RAW(16) NOT NULL,

	"ServiceContract" RAW(16) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "Organization"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "MaintenanceProgram"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	"Periodicity" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "Location"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "StatusOfTheEquipment"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "MaintenanceOperation"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	"MaintenanceProgram" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "Periodicity"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "ScheduledMaintenanceOperation"
(

	"primaryKey" RAW(16) NOT NULL,

	"ExecutionDate" DATE NOT NULL,

	"MaintenanceOperation" RAW(16) NOT NULL,

	"MaintenancePlan" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "Contract"
(

	"primaryKey" RAW(16) NOT NULL,

	"Number" NVARCHAR2(255) NULL,

	"Date" DATE NOT NULL,

	"ValidityPeriod" DATE NULL,

	"Buyer" RAW(16) NOT NULL,

	"Seller" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "DocumentToTheModel"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" NVARCHAR2(255) NOT NULL,

	"FileReference" NVARCHAR2(255) NOT NULL,

	"EquipmentModel" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMNETLOCKDATA"
(

	"LockKey" NVARCHAR2(300) NOT NULL,

	"UserName" NVARCHAR2(300) NOT NULL,

	"LockDate" DATE NULL,

	 PRIMARY KEY ("LockKey")
) ;


CREATE TABLE "STORMSETTINGS"
(

	"primaryKey" RAW(16) NOT NULL,

	"Module" nvarchar2(1000) NULL,

	"Name" nvarchar2(255) NULL,

	"Value" CLOB NULL,

	"User" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMAdvLimit"
(

	"primaryKey" RAW(16) NOT NULL,

	"User" nvarchar2(255) NULL,

	"Published" NUMBER(1) NULL,

	"Module" nvarchar2(255) NULL,

	"Name" nvarchar2(255) NULL,

	"Value" CLOB NULL,

	"HotKeyData" NUMBER(10) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMFILTERSETTING"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" nvarchar2(255) NOT NULL,

	"DataObjectView" nvarchar2(255) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMWEBSEARCH"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" nvarchar2(255) NOT NULL,

	"Order" NUMBER(10) NOT NULL,

	"PresentView" nvarchar2(255) NOT NULL,

	"DetailedView" nvarchar2(255) NOT NULL,

	"FilterSetting_m0" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMFILTERDETAIL"
(

	"primaryKey" RAW(16) NOT NULL,

	"Caption" nvarchar2(255) NOT NULL,

	"DataObjectView" nvarchar2(255) NOT NULL,

	"ConnectMasterProp" nvarchar2(255) NOT NULL,

	"OwnerConnectProp" nvarchar2(255) NULL,

	"FilterSetting_m0" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMFILTERLOOKUP"
(

	"primaryKey" RAW(16) NOT NULL,

	"DataObjectType" nvarchar2(255) NOT NULL,

	"Container" nvarchar2(255) NULL,

	"ContainerTag" nvarchar2(255) NULL,

	"FieldsToView" nvarchar2(255) NULL,

	"FilterSetting_m0" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "UserSetting"
(

	"primaryKey" RAW(16) NOT NULL,

	"AppName" nvarchar2(256) NULL,

	"UserName" nvarchar2(512) NULL,

	"UserGuid" RAW(16) NULL,

	"ModuleName" nvarchar2(1024) NULL,

	"ModuleGuid" RAW(16) NULL,

	"SettName" nvarchar2(256) NULL,

	"SettGuid" RAW(16) NULL,

	"SettLastAccessTime" DATE NULL,

	"StrVal" nvarchar2(256) NULL,

	"TxtVal" CLOB NULL,

	"IntVal" NUMBER(10) NULL,

	"BoolVal" NUMBER(1) NULL,

	"GuidVal" RAW(16) NULL,

	"DecimalVal" NUMBER(20,10) NULL,

	"DateTimeVal" DATE NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "ApplicationLog"
(

	"primaryKey" RAW(16) NOT NULL,

	"Category" nvarchar2(64) NULL,

	"EventId" NUMBER(10) NULL,

	"Priority" NUMBER(10) NULL,

	"Severity" nvarchar2(32) NULL,

	"Title" nvarchar2(256) NULL,

	"Timestamp" DATE NULL,

	"MachineName" nvarchar2(32) NULL,

	"AppDomainName" nvarchar2(512) NULL,

	"ProcessId" nvarchar2(256) NULL,

	"ProcessName" nvarchar2(512) NULL,

	"ThreadName" nvarchar2(512) NULL,

	"Win32ThreadId" nvarchar2(128) NULL,

	"Message" nvarchar2(2000) NULL,

	"FormattedMessage" nvarchar2(2000) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMAG"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" nvarchar2(80) NOT NULL,

	"Login" nvarchar2(50) NULL,

	"Pwd" nvarchar2(50) NULL,

	"IsUser" NUMBER(1) NOT NULL,

	"IsGroup" NUMBER(1) NOT NULL,

	"IsRole" NUMBER(1) NOT NULL,

	"ConnString" nvarchar2(255) NULL,

	"Enabled" NUMBER(1) NULL,

	"Email" nvarchar2(80) NULL,

	"Comment" CLOB NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMLG"
(

	"primaryKey" RAW(16) NOT NULL,

	"Group_m0" RAW(16) NOT NULL,

	"User_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMAuObjType"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" nvarchar2(255) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMAuEntity"
(

	"primaryKey" RAW(16) NOT NULL,

	"ObjectPrimaryKey" nvarchar2(38) NOT NULL,

	"OperationTime" DATE NOT NULL,

	"OperationType" nvarchar2(100) NOT NULL,

	"ExecutionResult" nvarchar2(12) NOT NULL,

	"Source" nvarchar2(255) NOT NULL,

	"SerializedField" nvarchar2(2000) NULL,

	"User_m0" RAW(16) NOT NULL,

	"ObjectType_m0" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMAuField"
(

	"primaryKey" RAW(16) NOT NULL,

	"Field" nvarchar2(100) NOT NULL,

	"OldValue" nvarchar2(2000) NULL,

	"NewValue" nvarchar2(2000) NULL,

	"MainChange_m0" RAW(16) NULL,

	"AuditEntity_m0" RAW(16) NOT NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMI"
(

	"primaryKey" RAW(16) NOT NULL,

	"User_m0" RAW(16) NOT NULL,

	"Agent_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "Session"
(

	"primaryKey" RAW(16) NOT NULL,

	"UserKey" RAW(16) NULL,

	"StartedAt" DATE NULL,

	"LastAccess" DATE NULL,

	"Closed" NUMBER(1) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMS"
(

	"primaryKey" RAW(16) NOT NULL,

	"Name" nvarchar2(100) NOT NULL,

	"Type" nvarchar2(100) NULL,

	"IsAttribute" NUMBER(1) NOT NULL,

	"IsOperation" NUMBER(1) NOT NULL,

	"IsView" NUMBER(1) NOT NULL,

	"IsClass" NUMBER(1) NOT NULL,

	"SharedOper" NUMBER(1) NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	"Comment" CLOB NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMP"
(

	"primaryKey" RAW(16) NOT NULL,

	"Subject_m0" RAW(16) NOT NULL,

	"Agent_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMF"
(

	"primaryKey" RAW(16) NOT NULL,

	"FilterText" CLOB NULL,

	"Name" nvarchar2(255) NULL,

	"FilterTypeNView" nvarchar2(255) NULL,

	"Subject_m0" RAW(16) NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMAC"
(

	"primaryKey" RAW(16) NOT NULL,

	"TypeAccess" nvarchar2(7) NULL,

	"Filter_m0" RAW(16) NULL,

	"Permition_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMLO"
(

	"primaryKey" RAW(16) NOT NULL,

	"Class_m0" RAW(16) NOT NULL,

	"Operation_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMLA"
(

	"primaryKey" RAW(16) NOT NULL,

	"View_m0" RAW(16) NOT NULL,

	"Attribute_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMLV"
(

	"primaryKey" RAW(16) NOT NULL,

	"Class_m0" RAW(16) NOT NULL,

	"View_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;


CREATE TABLE "STORMLR"
(

	"primaryKey" RAW(16) NOT NULL,

	"StartDate" DATE NULL,

	"EndDate" DATE NULL,

	"Agent_m0" RAW(16) NOT NULL,

	"Role_m0" RAW(16) NOT NULL,

	"CreateTime" DATE NULL,

	"Creator" nvarchar2(255) NULL,

	"EditTime" DATE NULL,

	"Editor" nvarchar2(255) NULL,

	 PRIMARY KEY ("primaryKey")
) ;



ALTER TABLE "EquipmentModel"
	ADD CONSTRAINT "EquipmentModel_FOrganization_0" FOREIGN KEY ("Manufacturer") REFERENCES "Organization" ("primaryKey");

CREATE INDEX "EquipmentModel_IManufacturer" on "EquipmentModel" ("Manufacturer");

ALTER TABLE "MaintenancePlan"
	ADD CONSTRAINT "MaintenancePlan_FEquipment_0" FOREIGN KEY ("Equipment") REFERENCES "Equipment" ("primaryKey");

CREATE INDEX "MaintenancePlan_IEquipment" on "MaintenancePlan" ("Equipment");

ALTER TABLE "PurposeOfTheMaintenanceModel"
	ADD CONSTRAINT "PurposeOfTheMaintenanceMo_1985" FOREIGN KEY ("EquipmentModel") REFERENCES "EquipmentModel" ("primaryKey");

CREATE INDEX "PurposeOfTheMaintenanceMo_6258" on "PurposeOfTheMaintenanceModel" ("EquipmentModel");

ALTER TABLE "PurposeOfTheMaintenanceModel"
	ADD CONSTRAINT "PurposeOfTheMaintenanceMo_6627" FOREIGN KEY ("MaintenanceProgram") REFERENCES "MaintenanceProgram" ("primaryKey");

CREATE INDEX "PurposeOfTheMaintenanceMo_4114" on "PurposeOfTheMaintenanceModel" ("MaintenanceProgram");

ALTER TABLE "FactOperationOfTheMaintenance"
	ADD CONSTRAINT "FactOperationOfTheMainten_5535" FOREIGN KEY ("ScheduledMaintenanceOperation") REFERENCES "ScheduledMaintenanceOperation" ("primaryKey");

CREATE INDEX "FactOperationOfTheMainten_3553" on "FactOperationOfTheMaintenance" ("ScheduledMaintenanceOperation");

ALTER TABLE "FactOperationOfTheMaintenance"
	ADD CONSTRAINT "FactOperationOfTheMainten_1949" FOREIGN KEY ("MaintenanceOperation") REFERENCES "MaintenanceOperation" ("primaryKey");

CREATE INDEX "FactOperationOfTheMainten_4574" on "FactOperationOfTheMaintenance" ("MaintenanceOperation");

ALTER TABLE "FactOperationOfTheMaintenance"
	ADD CONSTRAINT "FactOperationOfTheMainten_9142" FOREIGN KEY ("FactOfTheMaintenance") REFERENCES "FactOfTheMaintenance" ("primaryKey");

CREATE INDEX "FactOperationOfTheMainten_4059" on "FactOperationOfTheMaintenance" ("FactOfTheMaintenance");

ALTER TABLE "FactOfTheMaintenance"
	ADD CONSTRAINT "FactOfTheMaintenance_FMai_5752" FOREIGN KEY ("MaintenancePlan") REFERENCES "MaintenancePlan" ("primaryKey");

CREATE INDEX "FactOfTheMaintenance_IMai_2649" on "FactOfTheMaintenance" ("MaintenancePlan");

ALTER TABLE "FactOfTheMaintenance"
	ADD CONSTRAINT "FactOfTheMaintenance_FEqu_9388" FOREIGN KEY ("Equipment") REFERENCES "Equipment" ("primaryKey");

CREATE INDEX "FactOfTheMaintenance_IEqu_1987" on "FactOfTheMaintenance" ("Equipment");

ALTER TABLE "Equipment"
	ADD CONSTRAINT "Equipment_FEmployee_0" FOREIGN KEY ("Accountable") REFERENCES "Employee" ("primaryKey");

CREATE INDEX "Equipment_IAccountable" on "Equipment" ("Accountable");

ALTER TABLE "Equipment"
	ADD CONSTRAINT "Equipment_FContract_0" FOREIGN KEY ("SupplyContract") REFERENCES "Contract" ("primaryKey");

CREATE INDEX "Equipment_ISupplyContract" on "Equipment" ("SupplyContract");

ALTER TABLE "Equipment"
	ADD CONSTRAINT "Equipment_FEquipmentModel_0" FOREIGN KEY ("Model") REFERENCES "EquipmentModel" ("primaryKey");

CREATE INDEX "Equipment_IModel" on "Equipment" ("Model");

ALTER TABLE "Equipment"
	ADD CONSTRAINT "Equipment_FLocation_0" FOREIGN KEY ("Location") REFERENCES "Location" ("primaryKey");

CREATE INDEX "Equipment_ILocation" on "Equipment" ("Location");

ALTER TABLE "Equipment"
	ADD CONSTRAINT "Equipment_FStatusOfTheEqu_6613" FOREIGN KEY ("Status") REFERENCES "StatusOfTheEquipment" ("primaryKey");

CREATE INDEX "Equipment_IStatus" on "Equipment" ("Status");

ALTER TABLE "Equipment"
	ADD CONSTRAINT "Equipment_FTypeOfEquipment_0" FOREIGN KEY ("Type") REFERENCES "TypeOfEquipment" ("primaryKey");

CREATE INDEX "Equipment_IType" on "Equipment" ("Type");

ALTER TABLE "Equipment"
	ADD CONSTRAINT "Equipment_FContract_1" FOREIGN KEY ("ServiceContract") REFERENCES "Contract" ("primaryKey");

CREATE INDEX "Equipment_IServiceContract" on "Equipment" ("ServiceContract");

ALTER TABLE "MaintenanceProgram"
	ADD CONSTRAINT "MaintenanceProgram_FPerio_4227" FOREIGN KEY ("Periodicity") REFERENCES "Periodicity" ("primaryKey");

CREATE INDEX "MaintenanceProgram_IPerio_6582" on "MaintenanceProgram" ("Periodicity");

ALTER TABLE "MaintenanceOperation"
	ADD CONSTRAINT "MaintenanceOperation_FMai_4962" FOREIGN KEY ("MaintenanceProgram") REFERENCES "MaintenanceProgram" ("primaryKey");

CREATE INDEX "MaintenanceOperation_IMai_2113" on "MaintenanceOperation" ("MaintenanceProgram");

ALTER TABLE "ScheduledMaintenanceOperation"
	ADD CONSTRAINT "ScheduledMaintenanceOpera_3635" FOREIGN KEY ("MaintenanceOperation") REFERENCES "MaintenanceOperation" ("primaryKey");

CREATE INDEX "ScheduledMaintenanceOpera_3517" on "ScheduledMaintenanceOperation" ("MaintenanceOperation");

ALTER TABLE "ScheduledMaintenanceOperation"
	ADD CONSTRAINT "ScheduledMaintenanceOpera_3316" FOREIGN KEY ("MaintenancePlan") REFERENCES "MaintenancePlan" ("primaryKey");

CREATE INDEX "ScheduledMaintenanceOpera_7132" on "ScheduledMaintenanceOperation" ("MaintenancePlan");

ALTER TABLE "Contract"
	ADD CONSTRAINT "Contract_FOrganization_0" FOREIGN KEY ("Buyer") REFERENCES "Organization" ("primaryKey");

CREATE INDEX "Contract_IBuyer" on "Contract" ("Buyer");

ALTER TABLE "Contract"
	ADD CONSTRAINT "Contract_FOrganization_1" FOREIGN KEY ("Seller") REFERENCES "Organization" ("primaryKey");

CREATE INDEX "Contract_ISeller" on "Contract" ("Seller");

ALTER TABLE "DocumentToTheModel"
	ADD CONSTRAINT "DocumentToTheModel_FEquip_9540" FOREIGN KEY ("EquipmentModel") REFERENCES "EquipmentModel" ("primaryKey");

CREATE INDEX "DocumentToTheModel_IEquip_4970" on "DocumentToTheModel" ("EquipmentModel");

ALTER TABLE "STORMWEBSEARCH"
	ADD CONSTRAINT "STORMWEBSEARCH_FSTORMFILT_6521" FOREIGN KEY ("FilterSetting_m0") REFERENCES "STORMFILTERSETTING" ("primaryKey");

ALTER TABLE "STORMFILTERDETAIL"
	ADD CONSTRAINT "STORMFILTERDETAIL_FSTORMF_2900" FOREIGN KEY ("FilterSetting_m0") REFERENCES "STORMFILTERSETTING" ("primaryKey");

ALTER TABLE "STORMFILTERLOOKUP"
	ADD CONSTRAINT "STORMFILTERLOOKUP_FSTORMF_1583" FOREIGN KEY ("FilterSetting_m0") REFERENCES "STORMFILTERSETTING" ("primaryKey");

ALTER TABLE "STORMLG"
	ADD CONSTRAINT "STORMLG_FSTORMAG_0" FOREIGN KEY ("Group_m0") REFERENCES "STORMAG" ("primaryKey");

ALTER TABLE "STORMLG"
	ADD CONSTRAINT "STORMLG_FSTORMAG_1" FOREIGN KEY ("User_m0") REFERENCES "STORMAG" ("primaryKey");

ALTER TABLE "STORMAuEntity"
	ADD CONSTRAINT "STORMAuEntity_FSTORMAG_0" FOREIGN KEY ("User_m0") REFERENCES "STORMAG" ("primaryKey");

ALTER TABLE "STORMAuEntity"
	ADD CONSTRAINT "STORMAuEntity_FSTORMAuObj_3287" FOREIGN KEY ("ObjectType_m0") REFERENCES "STORMAuObjType" ("primaryKey");

ALTER TABLE "STORMAuField"
	ADD CONSTRAINT "STORMAuField_FSTORMAuField_0" FOREIGN KEY ("MainChange_m0") REFERENCES "STORMAuField" ("primaryKey");

ALTER TABLE "STORMAuField"
	ADD CONSTRAINT "STORMAuField_FSTORMAuEntity_0" FOREIGN KEY ("AuditEntity_m0") REFERENCES "STORMAuEntity" ("primaryKey");

ALTER TABLE "STORMI"
	ADD CONSTRAINT "STORMI_FSTORMAG_0" FOREIGN KEY ("User_m0") REFERENCES "STORMAG" ("primaryKey");

ALTER TABLE "STORMI"
	ADD CONSTRAINT "STORMI_FSTORMAG_1" FOREIGN KEY ("Agent_m0") REFERENCES "STORMAG" ("primaryKey");

ALTER TABLE "STORMP"
	ADD CONSTRAINT "STORMP_FSTORMS_0" FOREIGN KEY ("Subject_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMP"
	ADD CONSTRAINT "STORMP_FSTORMAG_0" FOREIGN KEY ("Agent_m0") REFERENCES "STORMAG" ("primaryKey");

ALTER TABLE "STORMF"
	ADD CONSTRAINT "STORMF_FSTORMS_0" FOREIGN KEY ("Subject_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMAC"
	ADD CONSTRAINT "STORMAC_FSTORMF_0" FOREIGN KEY ("Filter_m0") REFERENCES "STORMF" ("primaryKey");

ALTER TABLE "STORMAC"
	ADD CONSTRAINT "STORMAC_FSTORMP_0" FOREIGN KEY ("Permition_m0") REFERENCES "STORMP" ("primaryKey");

ALTER TABLE "STORMLO"
	ADD CONSTRAINT "STORMLO_FSTORMS_0" FOREIGN KEY ("Class_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMLO"
	ADD CONSTRAINT "STORMLO_FSTORMS_1" FOREIGN KEY ("Operation_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMLA"
	ADD CONSTRAINT "STORMLA_FSTORMS_0" FOREIGN KEY ("View_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMLA"
	ADD CONSTRAINT "STORMLA_FSTORMS_1" FOREIGN KEY ("Attribute_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMLV"
	ADD CONSTRAINT "STORMLV_FSTORMS_0" FOREIGN KEY ("Class_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMLV"
	ADD CONSTRAINT "STORMLV_FSTORMS_1" FOREIGN KEY ("View_m0") REFERENCES "STORMS" ("primaryKey");

ALTER TABLE "STORMLR"
	ADD CONSTRAINT "STORMLR_FSTORMAG_0" FOREIGN KEY ("Agent_m0") REFERENCES "STORMAG" ("primaryKey");

ALTER TABLE "STORMLR"
	ADD CONSTRAINT "STORMLR_FSTORMAG_1" FOREIGN KEY ("Role_m0") REFERENCES "STORMAG" ("primaryKey");



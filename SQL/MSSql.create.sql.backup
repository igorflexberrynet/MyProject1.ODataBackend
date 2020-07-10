



CREATE TABLE [Employee] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Surname] NVARCHAR(MAX)  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 [Patronymic] NVARCHAR(MAX)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [EquipmentModel] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 [Manufacturer] UNIQUEIDENTIFIER  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [TypeOfEquipment] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [MaintenancePlan] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [StartDate] DATETIME  NULL,

	 [EndDate] DATETIME  NULL,

	 [Equipment] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [PurposeOfTheMaintenanceModel] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [EquipmentModel] UNIQUEIDENTIFIER  NOT NULL,

	 [MaintenanceProgram] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [FactOperationOfTheMaintenance] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [ExecutionDate] DATETIME  NOT NULL,

	 [Successfully] BIT  NOT NULL,

	 [ScheduledMaintenanceOperation] UNIQUEIDENTIFIER  NULL,

	 [MaintenanceOperation] UNIQUEIDENTIFIER  NOT NULL,

	 [FactOfTheMaintenance] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [FactOfTheMaintenance] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [StartDate] DATETIME  NULL,

	 [EndDate] DATETIME  NULL,

	 [ScanProtocol] NVARCHAR(MAX)  NULL,

	 [MaintenancePlan] UNIQUEIDENTIFIER  NULL,

	 [Equipment] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [Equipment] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NULL,

	 [ProductionDate] DATETIME  NULL,

	 [DateOfCommissioning] DATETIME  NULL,

	 [WarrantyPeriod] DATETIME  NULL,

	 [OperatingTime] INT  NULL,

	 [RunDate] DATETIME  NULL,

	 [Description] NVARCHAR(MAX)  NULL,

	 [Accountable] UNIQUEIDENTIFIER  NOT NULL,

	 [SupplyContract] UNIQUEIDENTIFIER  NULL,

	 [Model] UNIQUEIDENTIFIER  NOT NULL,

	 [Location] UNIQUEIDENTIFIER  NOT NULL,

	 [Status] UNIQUEIDENTIFIER  NOT NULL,

	 [Type] UNIQUEIDENTIFIER  NOT NULL,

	 [ServiceContract] UNIQUEIDENTIFIER  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [Organization] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [MaintenanceProgram] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 [Periodicity] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [Location] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [StatusOfTheEquipment] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [MaintenanceOperation] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 [MaintenanceProgram] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [Periodicity] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [ScheduledMaintenanceOperation] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [ExecutionDate] DATETIME  NOT NULL,

	 [MaintenanceOperation] UNIQUEIDENTIFIER  NOT NULL,

	 [MaintenancePlan] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [Contract] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Number] NVARCHAR(MAX)  NULL,

	 [Date] DATETIME  NOT NULL,

	 [ValidityPeriod] DATETIME  NULL,

	 [Buyer] UNIQUEIDENTIFIER  NOT NULL,

	 [Seller] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [DocumentToTheModel] (

	 [primaryKey] UNIQUEIDENTIFIER  NOT NULL,

	 [Name] NVARCHAR(MAX)  NOT NULL,

	 [FileReference] NVARCHAR(MAX)  NOT NULL,

	 [EquipmentModel] UNIQUEIDENTIFIER  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMNETLOCKDATA] (

	 [LockKey] VARCHAR(300)  NOT NULL,

	 [UserName] VARCHAR(300)  NOT NULL,

	 [LockDate] DATETIME  NULL,

	 PRIMARY KEY ([LockKey]))


CREATE TABLE [STORMSETTINGS] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Module] varchar(1000)  NULL,

	 [Name] varchar(255)  NULL,

	 [Value] text  NULL,

	 [User] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMAdvLimit] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [User] varchar(255)  NULL,

	 [Published] bit  NULL,

	 [Module] varchar(255)  NULL,

	 [Name] varchar(255)  NULL,

	 [Value] text  NULL,

	 [HotKeyData] int  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMFILTERSETTING] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Name] varchar(255)  NOT NULL,

	 [DataObjectView] varchar(255)  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMWEBSEARCH] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Name] varchar(255)  NOT NULL,

	 [Order] INT  NOT NULL,

	 [PresentView] varchar(255)  NOT NULL,

	 [DetailedView] varchar(255)  NOT NULL,

	 [FilterSetting_m0] uniqueidentifier  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMFILTERDETAIL] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Caption] varchar(255)  NOT NULL,

	 [DataObjectView] varchar(255)  NOT NULL,

	 [ConnectMasterProp] varchar(255)  NOT NULL,

	 [OwnerConnectProp] varchar(255)  NULL,

	 [FilterSetting_m0] uniqueidentifier  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMFILTERLOOKUP] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [DataObjectType] varchar(255)  NOT NULL,

	 [Container] varchar(255)  NULL,

	 [ContainerTag] varchar(255)  NULL,

	 [FieldsToView] varchar(255)  NULL,

	 [FilterSetting_m0] uniqueidentifier  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [UserSetting] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [AppName] varchar(256)  NULL,

	 [UserName] varchar(512)  NULL,

	 [UserGuid] uniqueidentifier  NULL,

	 [ModuleName] varchar(1024)  NULL,

	 [ModuleGuid] uniqueidentifier  NULL,

	 [SettName] varchar(256)  NULL,

	 [SettGuid] uniqueidentifier  NULL,

	 [SettLastAccessTime] DATETIME  NULL,

	 [StrVal] varchar(256)  NULL,

	 [TxtVal] varchar(max)  NULL,

	 [IntVal] int  NULL,

	 [BoolVal] bit  NULL,

	 [GuidVal] uniqueidentifier  NULL,

	 [DecimalVal] decimal(20,10)  NULL,

	 [DateTimeVal] DATETIME  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [ApplicationLog] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Category] varchar(64)  NULL,

	 [EventId] INT  NULL,

	 [Priority] INT  NULL,

	 [Severity] varchar(32)  NULL,

	 [Title] varchar(256)  NULL,

	 [Timestamp] DATETIME  NULL,

	 [MachineName] varchar(32)  NULL,

	 [AppDomainName] varchar(512)  NULL,

	 [ProcessId] varchar(256)  NULL,

	 [ProcessName] varchar(512)  NULL,

	 [ThreadName] varchar(512)  NULL,

	 [Win32ThreadId] varchar(128)  NULL,

	 [Message] varchar(2500)  NULL,

	 [FormattedMessage] varchar(max)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMAG] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Name] varchar(80)  NOT NULL,

	 [Login] varchar(50)  NULL,

	 [Pwd] varchar(50)  NULL,

	 [IsUser] bit  NOT NULL,

	 [IsGroup] bit  NOT NULL,

	 [IsRole] bit  NOT NULL,

	 [ConnString] varchar(255)  NULL,

	 [Enabled] bit  NULL,

	 [Email] varchar(80)  NULL,

	 [Comment] varchar(MAX)  NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMLG] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Group_m0] uniqueidentifier  NOT NULL,

	 [User_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMAuObjType] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Name] nvarchar(255)  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMAuEntity] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [ObjectPrimaryKey] nvarchar(38)  NOT NULL,

	 [OperationTime] DATETIME  NOT NULL,

	 [OperationType] nvarchar(100)  NOT NULL,

	 [ExecutionResult] nvarchar(12)  NOT NULL,

	 [Source] nvarchar(255)  NOT NULL,

	 [SerializedField] nvarchar(max)  NULL,

	 [User_m0] uniqueidentifier  NOT NULL,

	 [ObjectType_m0] uniqueidentifier  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMAuField] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Field] nvarchar(100)  NOT NULL,

	 [OldValue] nvarchar(max)  NULL,

	 [NewValue] nvarchar(max)  NULL,

	 [MainChange_m0] uniqueidentifier  NULL,

	 [AuditEntity_m0] uniqueidentifier  NOT NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMI] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [User_m0] uniqueidentifier  NOT NULL,

	 [Agent_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [Session] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [UserKey] uniqueidentifier  NULL,

	 [StartedAt] datetime  NULL,

	 [LastAccess] datetime  NULL,

	 [Closed] bit  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMS] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Name] varchar(100)  NOT NULL,

	 [Type] varchar(100)  NULL,

	 [IsAttribute] bit  NOT NULL,

	 [IsOperation] bit  NOT NULL,

	 [IsView] bit  NOT NULL,

	 [IsClass] bit  NOT NULL,

	 [SharedOper] bit  NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 [Comment] varchar(MAX)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMP] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Subject_m0] uniqueidentifier  NOT NULL,

	 [Agent_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMF] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [FilterText] varchar(MAX)  NULL,

	 [Name] varchar(255)  NULL,

	 [FilterTypeNView] varchar(255)  NULL,

	 [Subject_m0] uniqueidentifier  NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMAC] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [TypeAccess] varchar(7)  NULL,

	 [Filter_m0] uniqueidentifier  NULL,

	 [Permition_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMLO] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Class_m0] uniqueidentifier  NOT NULL,

	 [Operation_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMLA] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [View_m0] uniqueidentifier  NOT NULL,

	 [Attribute_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMLV] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [Class_m0] uniqueidentifier  NOT NULL,

	 [View_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))


CREATE TABLE [STORMLR] (

	 [primaryKey] uniqueidentifier  NOT NULL,

	 [StartDate] datetime  NULL,

	 [EndDate] datetime  NULL,

	 [Agent_m0] uniqueidentifier  NOT NULL,

	 [Role_m0] uniqueidentifier  NOT NULL,

	 [CreateTime] datetime  NULL,

	 [Creator] varchar(255)  NULL,

	 [EditTime] datetime  NULL,

	 [Editor] varchar(255)  NULL,

	 PRIMARY KEY ([primaryKey]))




 ALTER TABLE [EquipmentModel] ADD CONSTRAINT [EquipmentModel_FOrganization_0] FOREIGN KEY ([Manufacturer]) REFERENCES [Organization]
CREATE INDEX EquipmentModel_IManufacturer on [EquipmentModel] ([Manufacturer])

 ALTER TABLE [MaintenancePlan] ADD CONSTRAINT [MaintenancePlan_FEquipment_0] FOREIGN KEY ([Equipment]) REFERENCES [Equipment]
CREATE INDEX MaintenancePlan_IEquipment on [MaintenancePlan] ([Equipment])

 ALTER TABLE [PurposeOfTheMaintenanceModel] ADD CONSTRAINT [PurposeOfTheMaintenanceModel_FEquipmentModel_0] FOREIGN KEY ([EquipmentModel]) REFERENCES [EquipmentModel]
CREATE INDEX PurposeOfTheMaintenanceModel_IEquipmentModel on [PurposeOfTheMaintenanceModel] ([EquipmentModel])

 ALTER TABLE [PurposeOfTheMaintenanceModel] ADD CONSTRAINT [PurposeOfTheMaintenanceModel_FMaintenanceProgram_0] FOREIGN KEY ([MaintenanceProgram]) REFERENCES [MaintenanceProgram]
CREATE INDEX PurposeOfTheMaintenanceModel_IMaintenanceProgram on [PurposeOfTheMaintenanceModel] ([MaintenanceProgram])

 ALTER TABLE [FactOperationOfTheMaintenance] ADD CONSTRAINT [FactOperationOfTheMaintenance_FScheduledMaintenanceOperation_0] FOREIGN KEY ([ScheduledMaintenanceOperation]) REFERENCES [ScheduledMaintenanceOperation]
CREATE INDEX FactOperationOfTheMaintenance_IScheduledMaintenanceOperation on [FactOperationOfTheMaintenance] ([ScheduledMaintenanceOperation])

 ALTER TABLE [FactOperationOfTheMaintenance] ADD CONSTRAINT [FactOperationOfTheMaintenance_FMaintenanceOperation_0] FOREIGN KEY ([MaintenanceOperation]) REFERENCES [MaintenanceOperation]
CREATE INDEX FactOperationOfTheMaintenance_IMaintenanceOperation on [FactOperationOfTheMaintenance] ([MaintenanceOperation])

 ALTER TABLE [FactOperationOfTheMaintenance] ADD CONSTRAINT [FactOperationOfTheMaintenance_FFactOfTheMaintenance_0] FOREIGN KEY ([FactOfTheMaintenance]) REFERENCES [FactOfTheMaintenance]
CREATE INDEX FactOperationOfTheMaintenance_IFactOfTheMaintenance on [FactOperationOfTheMaintenance] ([FactOfTheMaintenance])

 ALTER TABLE [FactOfTheMaintenance] ADD CONSTRAINT [FactOfTheMaintenance_FMaintenancePlan_0] FOREIGN KEY ([MaintenancePlan]) REFERENCES [MaintenancePlan]
CREATE INDEX FactOfTheMaintenance_IMaintenancePlan on [FactOfTheMaintenance] ([MaintenancePlan])

 ALTER TABLE [FactOfTheMaintenance] ADD CONSTRAINT [FactOfTheMaintenance_FEquipment_0] FOREIGN KEY ([Equipment]) REFERENCES [Equipment]
CREATE INDEX FactOfTheMaintenance_IEquipment on [FactOfTheMaintenance] ([Equipment])

 ALTER TABLE [Equipment] ADD CONSTRAINT [Equipment_FEmployee_0] FOREIGN KEY ([Accountable]) REFERENCES [Employee]
CREATE INDEX Equipment_IAccountable on [Equipment] ([Accountable])

 ALTER TABLE [Equipment] ADD CONSTRAINT [Equipment_FContract_0] FOREIGN KEY ([SupplyContract]) REFERENCES [Contract]
CREATE INDEX Equipment_ISupplyContract on [Equipment] ([SupplyContract])

 ALTER TABLE [Equipment] ADD CONSTRAINT [Equipment_FEquipmentModel_0] FOREIGN KEY ([Model]) REFERENCES [EquipmentModel]
CREATE INDEX Equipment_IModel on [Equipment] ([Model])

 ALTER TABLE [Equipment] ADD CONSTRAINT [Equipment_FLocation_0] FOREIGN KEY ([Location]) REFERENCES [Location]
CREATE INDEX Equipment_ILocation on [Equipment] ([Location])

 ALTER TABLE [Equipment] ADD CONSTRAINT [Equipment_FStatusOfTheEquipment_0] FOREIGN KEY ([Status]) REFERENCES [StatusOfTheEquipment]
CREATE INDEX Equipment_IStatus on [Equipment] ([Status])

 ALTER TABLE [Equipment] ADD CONSTRAINT [Equipment_FTypeOfEquipment_0] FOREIGN KEY ([Type]) REFERENCES [TypeOfEquipment]
CREATE INDEX Equipment_IType on [Equipment] ([Type])

 ALTER TABLE [Equipment] ADD CONSTRAINT [Equipment_FContract_1] FOREIGN KEY ([ServiceContract]) REFERENCES [Contract]
CREATE INDEX Equipment_IServiceContract on [Equipment] ([ServiceContract])

 ALTER TABLE [MaintenanceProgram] ADD CONSTRAINT [MaintenanceProgram_FPeriodicity_0] FOREIGN KEY ([Periodicity]) REFERENCES [Periodicity]
CREATE INDEX MaintenanceProgram_IPeriodicity on [MaintenanceProgram] ([Periodicity])

 ALTER TABLE [MaintenanceOperation] ADD CONSTRAINT [MaintenanceOperation_FMaintenanceProgram_0] FOREIGN KEY ([MaintenanceProgram]) REFERENCES [MaintenanceProgram]
CREATE INDEX MaintenanceOperation_IMaintenanceProgram on [MaintenanceOperation] ([MaintenanceProgram])

 ALTER TABLE [ScheduledMaintenanceOperation] ADD CONSTRAINT [ScheduledMaintenanceOperation_FMaintenanceOperation_0] FOREIGN KEY ([MaintenanceOperation]) REFERENCES [MaintenanceOperation]
CREATE INDEX ScheduledMaintenanceOperation_IMaintenanceOperation on [ScheduledMaintenanceOperation] ([MaintenanceOperation])

 ALTER TABLE [ScheduledMaintenanceOperation] ADD CONSTRAINT [ScheduledMaintenanceOperation_FMaintenancePlan_0] FOREIGN KEY ([MaintenancePlan]) REFERENCES [MaintenancePlan]
CREATE INDEX ScheduledMaintenanceOperation_IMaintenancePlan on [ScheduledMaintenanceOperation] ([MaintenancePlan])

 ALTER TABLE [Contract] ADD CONSTRAINT [Contract_FOrganization_0] FOREIGN KEY ([Buyer]) REFERENCES [Organization]
CREATE INDEX Contract_IBuyer on [Contract] ([Buyer])

 ALTER TABLE [Contract] ADD CONSTRAINT [Contract_FOrganization_1] FOREIGN KEY ([Seller]) REFERENCES [Organization]
CREATE INDEX Contract_ISeller on [Contract] ([Seller])

 ALTER TABLE [DocumentToTheModel] ADD CONSTRAINT [DocumentToTheModel_FEquipmentModel_0] FOREIGN KEY ([EquipmentModel]) REFERENCES [EquipmentModel]
CREATE INDEX DocumentToTheModel_IEquipmentModel on [DocumentToTheModel] ([EquipmentModel])

 ALTER TABLE [STORMWEBSEARCH] ADD CONSTRAINT [STORMWEBSEARCH_FSTORMFILTERSETTING_0] FOREIGN KEY ([FilterSetting_m0]) REFERENCES [STORMFILTERSETTING]

 ALTER TABLE [STORMFILTERDETAIL] ADD CONSTRAINT [STORMFILTERDETAIL_FSTORMFILTERSETTING_0] FOREIGN KEY ([FilterSetting_m0]) REFERENCES [STORMFILTERSETTING]

 ALTER TABLE [STORMFILTERLOOKUP] ADD CONSTRAINT [STORMFILTERLOOKUP_FSTORMFILTERSETTING_0] FOREIGN KEY ([FilterSetting_m0]) REFERENCES [STORMFILTERSETTING]

 ALTER TABLE [STORMLG] ADD CONSTRAINT [STORMLG_FSTORMAG_0] FOREIGN KEY ([Group_m0]) REFERENCES [STORMAG]

 ALTER TABLE [STORMLG] ADD CONSTRAINT [STORMLG_FSTORMAG_1] FOREIGN KEY ([User_m0]) REFERENCES [STORMAG]

 ALTER TABLE [STORMAuEntity] ADD CONSTRAINT [STORMAuEntity_FSTORMAG_0] FOREIGN KEY ([User_m0]) REFERENCES [STORMAG]

 ALTER TABLE [STORMAuEntity] ADD CONSTRAINT [STORMAuEntity_FSTORMAuObjType_0] FOREIGN KEY ([ObjectType_m0]) REFERENCES [STORMAuObjType]

 ALTER TABLE [STORMAuField] ADD CONSTRAINT [STORMAuField_FSTORMAuField_0] FOREIGN KEY ([MainChange_m0]) REFERENCES [STORMAuField]

 ALTER TABLE [STORMAuField] ADD CONSTRAINT [STORMAuField_FSTORMAuEntity_0] FOREIGN KEY ([AuditEntity_m0]) REFERENCES [STORMAuEntity]

 ALTER TABLE [STORMI] ADD CONSTRAINT [STORMI_FSTORMAG_0] FOREIGN KEY ([User_m0]) REFERENCES [STORMAG]

 ALTER TABLE [STORMI] ADD CONSTRAINT [STORMI_FSTORMAG_1] FOREIGN KEY ([Agent_m0]) REFERENCES [STORMAG]

 ALTER TABLE [STORMP] ADD CONSTRAINT [STORMP_FSTORMS_0] FOREIGN KEY ([Subject_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMP] ADD CONSTRAINT [STORMP_FSTORMAG_0] FOREIGN KEY ([Agent_m0]) REFERENCES [STORMAG]

 ALTER TABLE [STORMF] ADD CONSTRAINT [STORMF_FSTORMS_0] FOREIGN KEY ([Subject_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMAC] ADD CONSTRAINT [STORMAC_FSTORMF_0] FOREIGN KEY ([Filter_m0]) REFERENCES [STORMF]

 ALTER TABLE [STORMAC] ADD CONSTRAINT [STORMAC_FSTORMP_0] FOREIGN KEY ([Permition_m0]) REFERENCES [STORMP]

 ALTER TABLE [STORMLO] ADD CONSTRAINT [STORMLO_FSTORMS_0] FOREIGN KEY ([Class_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMLO] ADD CONSTRAINT [STORMLO_FSTORMS_1] FOREIGN KEY ([Operation_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMLA] ADD CONSTRAINT [STORMLA_FSTORMS_0] FOREIGN KEY ([View_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMLA] ADD CONSTRAINT [STORMLA_FSTORMS_1] FOREIGN KEY ([Attribute_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMLV] ADD CONSTRAINT [STORMLV_FSTORMS_0] FOREIGN KEY ([Class_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMLV] ADD CONSTRAINT [STORMLV_FSTORMS_1] FOREIGN KEY ([View_m0]) REFERENCES [STORMS]

 ALTER TABLE [STORMLR] ADD CONSTRAINT [STORMLR_FSTORMAG_0] FOREIGN KEY ([Agent_m0]) REFERENCES [STORMAG]

 ALTER TABLE [STORMLR] ADD CONSTRAINT [STORMLR_FSTORMAG_1] FOREIGN KEY ([Role_m0]) REFERENCES [STORMAG]


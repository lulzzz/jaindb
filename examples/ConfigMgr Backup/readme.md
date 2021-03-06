ConfigMgr Objects:

| **Class**                                  | id                                   | QueryAll                                                                                                               |
|----------------------------------------|--------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| TaskSequence                           | ts-{PackageID}                       | http://localhost:5000/query?TaskSequence.Name                                                                          |
| App                                    | app-{PackageID}                      | http://localhost:5000/query?App.%23LocalizedDisplayName;App.AppMgmtDigest.DeploymentType..Title.value                  |
| App.AppMgmtDigest.DeploymentType       | app-{PackageID}                      | http://localhost:5000/query?App.AppMgmtDigest.DeploymentType                                                           |
| Collection                             | coll-{CollectionID}                  | http://loclahost:5000/query?Collection.%23Name                                                                         |
| CollectionSettings                     | coll-{CollectionID}; #CollectionID"" | http://localhost:5000/query?CollectionSettings.%23CollectionID&$select=CollectionSetting                               |
| CollectionSettings.ServiceWindows      | coll-{CollectionID}                  | http://localhost:5000/query?CollectionSettings.ServiceWindows.ServiceWindowID;CollectionSettings.ServiceWindows        |
| CollectionSettings.CollectionVariables | coll-{CollectionID}                  | http://localhost:5000/query?CollectionSettings.CollectionVariables..Name;CollectionSettings.CollectionVariables..Value |
| Package                                | pkg-{PackageID}                      | http://loclahost:5000/query?Package.Name                                                                               |
| Programs                               | pkg-{PackageID}                      | http://localhost:5000/query?Package.Name;Programs..ProgramName                                                         |
| BoundaryGroup                          | bg-{GroupID}                         | http://loclahost:5000/query?BoundaryGroup.Name                                                                         |
| Boundary                               | bip-{BoundaryID}                     | http://loclahost:5000/query?Boundary.BoundaryType;Boundary.Value                                                       |
| BoundaryRelationship                   | {hash}                               | http://loclahost:5000/query?BoundaryRelationship                                                                       |
| BootImage                              | boot-{PackageID}                     | http://localhost:5000/query?BootImage.Name                                                                             |
| ClientSettings                         | cfg-{SettingsID}                     | http://localhost:5000/query?ClientSettings.Name                                                                        |
| ConfigItem                             | ci-{CI_ID}                           | http://loclahost:5000/query?ConfigItem.LocalizedDisplayName;ConfigItem.CI_UniqueID                                     |
| Baseline                               | bl-{CI_ID}                           | http://localhost:5000/query?Baseline.LocalizedDisplayName;Baseline.CI_UniqueID                                         |
| SiteSystemServer                       | srv-{NetworkOSPath}                  | http://localhost:5000/query?SiteSystemServer.NetworkOSPath;SiteSystemServer.RoleName                                   |
| DistributionPointGroup                 | dpg-{GroupID}                        | http://localhost:5000/query?DistributionPointGroup.Name                                                                |
| DistributionPointInfo                  | dp-{ID}                              | http://localhost:5000/query?DistributionPointInfo.Name;DistributionPointInfo.IsPXE;DistributionPointInfo.IsActive      |
| HierarchySetting                       | site-{SiteCode}                      | http://localhost:5000/query?HierarchySetting.SiteName;HierarchySetting.SiteCode                                        |
| SiteMaintenanceTask                    | tsk-{ItemName}                       | http://localhost:5000/query?SiteMaintenanceTask.ItemName                                                               |
| SoftwareUpdate                         | upd-{CI_ID}                          | http://localhost:5000/query?SoftwareUpdate.ArticleID;SoftwareUpdate.LocalizedDisplayName                               |
| UpdateGroupDeployment                  | ugd-{AssignmentID}                   | http://localhost:5000/query?UpdateGroupDeployment.AssignmentName                                                       |
| Device                                 | res-{ResourceID}                     | http://localhost:5000/query?Device.Name                                                                                |
| DeviceVariable                         | res-{ResourceID}                     | http://localhost:5000/query?DeviceVariable..Name;DeviceVariable..Value                                                 |
| UserDeviceAffinity                     | res-{ResourceID}                     | http://localhost:5000/query?UserDeviceAffinity..ResourceName;UserDeviceAffinity..UniqueUserName                        |
| OperatingSystemUpgradePackage          | osd-{PackageID}                      | http://localhost:5000/query?OperatingSystemUpgradePackage.Name                                                         |
| OperatingSystemImage                   | osd-{PackageID}                      | http://localhost:5000/query?OperatingSystemImage.Name                                                                  |
| Deployment                             | depl-{DeploymentID}                  | http://localhost:5000/query?Deployment.CollectionName;Deployment.SoftwareName                                          |
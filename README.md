# DSCMgmtPack Version 1.1.0.0 (beta)

SCOM Management Pack for the DSC (Desired State Configuration) Projekt you will find here: https://github.com/dsccommunity/dscworkshop i

This Management-Pack monitores all managed SCOM Nodes for proper DSC configuration:

 - there is an Alerting for all SCOM monitored Agents which have no DSC configuration active
 - there is a View for all SCOM monitored agents which have a DSC configuration (Healthy) or not (Critical)
 - there is a View for the state monitoring of all DSC configured Agents which have a state of not equal healthy
 - there are Tasks for initial configuration of an SCOM Agent with DSC (overridable), for re-apply the configuration and a Task for Consistency-Check and Config-Pull
 
 Please be aware that we have here a beta status at the moment. So test this Managment-Pack first in your Test-Environment.
 
 This Managment Pack contains
 
  - CLASS DSC.ManagedNode.Seed.Claas
  - CLASS DSC.ManagedNode.IsManaged.Class
  - MONITOR DSC.ManagedNode.IsManaged.Monitor
  - TASK DSC.UnmanagedNode.InitialConfig.Task
  - TASK DSC.ManagedNode.IsManaged.ReApply.Configuration.Task
  - TASK DSC.ManagedNode.IsManaged.ConsistencyCheckAnd.ConfigPull.Task

Detailed documentation will be available soon.

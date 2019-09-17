# Experimental.System.Messaging
Experimental port of System.Messaging (for .NET Core)

## Introduction

This package is a counterfeit of the .NET Framework version System.Messaging assembly for .NET Core applications running on Windows Client and Windows Server. It is provided for development convenience. Do not use this package if Microsoft officially releases this package again. Also, once it is released, you should migrate the code to the new package.

The source code for this package is excerpted from the .NET Framework reference source code.

## Release Note

### v1.0.1 (17 September 2019)
I lifted some more code from the .NET Framework reference source in order to add support for MessageQueue.SetPermissions(...). Bear in mind, however, that some lines of code from the reference source has been removed in order to ease the process of implementing SetPermissions(...). As a result, this version may be insecure. Do not use in production.

### v1.0.0 (2018-01-06)
This version of the System.Messaging package excludes all advanced features such as code access security, execute permissions, and Active Directory integration. I released the package keeping in mind the minimal use of Message Queuing communication facilities. Please confirm whether it is suitable for actual use through unit test and integration test.

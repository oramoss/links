# Virtual Machine
Links related to Virtual Machine.

## Capabilities
- [Automanage VM](https://www.thomasmaurer.ch/2020/10/automanage-for-azure-virtual-machines/)
- [Announcing preview of Azure Trusted Launch for virtual machines](https://azure.microsoft.com/en-us/blog/announcing-preview-of-azure-trusted-launch-for-virtual-machines/)
- [How to add Azure virtual machines to inventory](https://abdulwkazi.com/2021/03/29/addvmstoinventory/)

## Extensions
- [IaaS AntiMalware, Windows](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/iaas-antimalware-windows)
- [Azure Disk Encryption](https://azsec.azurewebsites.net/2019/12/28/azure-disk-encryption-arm-template-for-windows-vm/)

- [Overview of Azure Monitor agents](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/agents-overview)
- [Azure Monitor agent overview](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-overview?tabs=PowerShellWindows)

- [DependencyAgent](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/agent-dependency-windows)
  - Azure Monitor Dependency Agent
  - Microsoft.Azure.Monitoring.DependencyAgent
  - Windows (DependencyAgentWindows)
  - Linux (DependencyAgentLinux)
- [Azure Monitor Agent (the future)](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-install?tabs=ARMAgentPowerShell%2CPowerShellWindows%2CPowerShellWindowsArc%2CCLIWindows%2CCLIWindowsArc)
  - Microsoft.Azure.Monitor
  - AzureMonitorWindowsAgent
  - AzureMonitorLinuxAgent
- CustomScriptExtension
  - ASC use this for TZ set
- [GuestConfigForWindows](https://azsec.azurewebsites.net/2020/03/22/arm-template-for-azure-vm-with-guest-configuration/)
  - https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/guest-configuration
  - The Guest Configuration extension is a component Azure Policy that performs audit and configuration operations inside virtual machines. Policies such as security baseline definitions for Linux and Windows can't check settings inside machines until the extension is installed.
- [GuestHealthWindowsAgent](https://docs.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-health-overview)
  - VM insights guest health allows you to view the health of virtual machines based on a set of performance measurements that are sampled at regular intervals from the guest operating system. You can quickly check the health of all virtual machines in a subscription or resource group, drill down on the detailed health of a particular virtual machine, or be proactively notified when a virtual machine becomes unhealthy.
- IaaSAntimalware
  - ASC use ESET instead so comment out
- joindomain
  - ASC use this for domain joining to advanced-processing.com
- [Microsoft.Insights.VMDiagnosticsSettings](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/diagnostics-template)
    - LAW Diagnostics logging
    - The Azure Diagnostics Extension provides the monitoring and diagnostics capabilities on a Windows-based Azure virtual machine.
- [MicrosoftMonitoringAgent](https://docs.microsoft.com/en-us/services-hub/health/mma-setup)
  - Azure Monitor Agent - the future for all monitoring - not there yet though so need to use combo of this and older agents for now
- SqlIaasExtension
  - SQL Virtual Machine 
  - Add to any VM used by SQL


Enable Health on VM leads to DependencyAgent/MicrosoftMonitoringAgent being installed
Add VM to DCR leads to AzureMonitorWindowsAgent being installed


## DR
- [Set up DR for IaaS VMs](https://techcommunity.microsoft.com/t5/itops-talk-blog/how-to-set-up-disaster-recovery-for-azure-iaas-vms/ba-p/1153807?WT.mc_id=twitter-social-thmaure)
- [About networking in Azure VM disaster recovery](https://docs.microsoft.com/en-us/azure/site-recovery/azure-to-azure-about-networking)
- [Tutorial: Fail over Azure VMs to a secondary region](https://docs.microsoft.com/en-us/azure/site-recovery/azure-to-azure-tutorial-failover-failback)
- [How to restore Azure VM data in Azure portal](https://docs.microsoft.com/en-us/azure/backup/backup-azure-arm-restore-vms#cross-region-restore)

## Windows
- [Error changing time zone in Windows Server 2019: Use the command line or PowerShell instead](https://4sysops.com/archives/error-changing-time-zone-in-windows-server-2019-use-the-command-line-or-powershell-instead/)
- [Changing Azure VM’s Default Locale](https://techdailychronicle.com/changing-azure-vms-default-locale/)

## Automation
- [Azure Data Factory Solution to Start and Stop VM](https://www.techtalkcorner.com/start-and-stop-azure-vm/)
- [Resource Manager template samples for agents in Azure Monitor](https://docs.microsoft.com/en-us/azure/azure-monitor/agents/resource-manager-agent)

## Miscellaneous
- [Azure VMs and disabling NLA on domain level](https://docs.microsoft.com/en-us/answers/questions/268781/azure-vms-and-disabling-nla-on-domain-level.html)
- [Run PowerShell scripts in your Windows VM by using Run Command](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/run-command#azure-portal)
- [Troubleshoot authentication errors when you use RDP to connect to Azure VM](https://docs.microsoft.com/en-us/troubleshoot/azure/virtual-machines/cannot-connect-rdp-azure-vm)
- [Moving your Azure Virtual Machines has never been easier!](https://azure.microsoft.com/en-ca/blog/moving-your-azure-virtual-machines-has-never-been-easier/)
- [Move Azure VMs into Availability Zones](https://docs.microsoft.com/en-us/azure/site-recovery/move-azure-vms-avset-azone)
- [Lost RDP Access due to Firewall - reset method via Portal    ](https://serverfault.com/questions/769768/lost-rdp-access-to-vm-azure-after-firewall-changes)
- [Optimizing VMs in Azure](https://virtualizationreview.com/articles/2018/08/07/optimizing-vms-in-azure.aspx)
- [ENABLING DISK ENCRYPTION ON VIRTUAL MACHINES IN AZURE](https://www.fredrikengseth.com/enabling-disk-encryption-on-virtual-machines-in-azure/)
- [Change VM Zone script](https://github.com/kpantos/azure-automation/blob/master/powershell/change-vm-zone.ps1)
- [Change All Windows Servers to TLS 1.2 with PowerShell!](https://www.shankuehn.io/post/change-all-windows-servers-to-tls-1-2-with-powershell)
- [How to run scripts against multiple Azure VMs by using Run Command](https://www.thomasmaurer.ch/2021/03/how-to-run-scripts-against-multiple-azure-vms-by-using-run-command/)

## Imaging
- [Creating An Azure VM From The VHDX/VHD File](https://www.c-sharpcorner.com/article/creating-an-azure-vm-from-the-vhdxvhd-file/)
- [How to Merge Hyper-V Snapshots: A Step-By-Step Guide](https://www.nakivo.com/hyper-v-backup/merge-hyper-v-snapshots-step-step-guide/)
- [Create a managed image of a generalized VM in Azure](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/capture-image-resource)
- [Prepare a Windows VHD or VHDX to upload to Azure](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/prepare-for-upload-vhd-image)
- [Create a WIM file from the WVD VHD file.](https://www.microcloud.nl/create-a-wim-file-from-the-wvd-vhd-file)
- [bginfo tool](https://docs.microsoft.com/en-us/sysinternals/downloads/bginfo)
- [How to Get a Windows 11 ISO File and Do a Clean Install](https://www.tomshardware.com/how-to/clean-install-windows-11)
- [Building VM Images Using Azure Image Builder](https://www.pluralsight.com/courses/building-vm-images-using-azure-image-builder)

## Desired State Configuration
- [Azure & Desired State Configuration Part 1/4](https://techcommunity.microsoft.com/t5/core-infrastructure-and-security/azure-amp-desired-state-configuration-part-1-4/ba-p/2609032)

## Hyper-V
- [Hyper-V Network Adapters: What, Why, and How](https://www.nakivo.com/blog/hyper-v-network-adapters-what-why-and-how/)

## Extensions
- [ARM template for Azure VM with Guest Configuration](https://azsec.azurewebsites.net/2020/03/22/arm-template-for-azure-vm-with-guest-configuration/)
- [Join a Windows Server virtual machine to an Azure Active Directory Domain Services managed domain using a Resource Manager template](https://docs.microsoft.com/en-us/azure/active-directory-domain-services/join-windows-vm-template)
- [Custom Script Extension for Windows](https://docs.microsoft.com/en-us/azure/virtual-machines/extensions/custom-script-windows)
- [Register SQL Server VM with SQL IaaS Agent Extension](https://docs.microsoft.com/en-us/azure/azure-sql/virtual-machines/windows/sql-agent-extension-manually-register-single-vm?tabs=bash%2Cazure-cli)

## Performance
- [Comparing Azure Premium and UltraSSD disks](https://blog.dirkallaert.be/2020/04/03/comparing-azure-premium-and-ultrassd-disks/#:~:text=In%20comparison%20with%20on-premise%20SSD%20based%20storage%20the,the%20neighborhood%20of%202-4ms%20when%20caching%20is%20disabled.)
- [Overview of Azure Virtual Machine IO performance and throttles](https://sabin.io/blog/overview-of-azure-virtual-machine-io-performance-and-throttles/)
- [Monitoring virtual machines with Azure Monitor](https://docs.microsoft.com/en-us/azure/azure-monitor/vm/monitor-virtual-machine?WT.mc_id=enterprise-0000-shkuehn)

## Security
- [What is the built-in vulnerability assessment tool in Azure Security Center?](https://techcommunity.microsoft.com/t5/azure-security-center/built-in-vulnerability-assessment-for-vms-in-azure-security/ba-p/1577947)

## SQL IaaS
- [Windows Server Failover Cluster with SQL Server on Azure VMs](https://docs.microsoft.com/en-us/azure/azure-sql/virtual-machines/windows/hadr-windows-server-failover-cluster-overview)

## Monitoring
- [Monitor scheduled events for your Azure VMs](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/scheduled-event-service)

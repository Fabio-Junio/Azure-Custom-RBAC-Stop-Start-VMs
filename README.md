# Azure Custom RBAC Stop-Start VMs

Assistam ao vídeo do canal Azure Xplorer para auxiliar na configuração e importação do seu arquivo JSON:
https://youtu.be/40W98RRsGwM

O arquivo JSON Virtual Machine Stop-Start.json pode ser util no seu ambiente de Azure para ser específico para um usuário somente realizar o Stop, Start e Deallocate das Virtual Machines.

No parâmetro: "assignableScopes": [
            "/providers/Microsoft.Management/managementGroups/HML"
        ],

Faça a substituição de acordo com os parâmetros abaixo:

Se for Management Group:
"/providers/Microsoft.Management/SEU_MANAGEMENT_GROUP"

Se for Subscription:
"/subscriptions/0a91d1d7...xxx....xxx...87393"

ou Resource Group.
"/subscriptions/0a91d1d7...xxx....xxx...87393/resourceGroups/rg-prd"

Importe esse script através do RBAC custom role na seu Management Group ou Subscription ou Resource Group e depois configure os usuários ou grupos que irão ter essa role atribuída.

##################

The JSON file Virtual Machine Stop-Start.json can be useful in your Azure environment to be specific to a user only to perform the Stop, Start and Deallocate of Virtual Machines.

Watch the video on the Azure Xplorer channel to help you configure and import your JSON file:
https://youtu.be/40W98RRsGwM


In the parameter: "assignableScopes": [
"/providers/Microsoft.Management/managementGroups/HML"
],

Make the replacement according to the parameters below:

If it is Management Group:
"/providers/Microsoft.Management/YOUR_MANAGEMENT_GROUP"

If it is Subscription:
"/subscriptions/0a91d1d7...xxx....xxx...87393"

or Resource Group.
"/subscriptions/0a91d1d7...xxx....xxx...87393/resourceGroups/rg-prd"

Import this script through the RBAC custom role in your Management Group or Subscription or Resource Group and then configure the users or groups that will have this role assigned.

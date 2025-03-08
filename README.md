# Azure RBAC-Personalized-Stop-Start-VMs
RBAC Personalized to Stop, Start and Deallocate VMs

Este scritp em json pode ser util no seu ambiente de Azure para ser específico para um usuário somente realizar o Stop, Start e Deallocate das Virtual Machines.

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

Importe esse script através do RBAC custom role e depois configure os usuários ou grupos que irão ter essa role atribuída.

##################

This JSON script can be useful in your Azure environment to be specific to a user only to perform Stop, Start and Deallocate of Virtual Machines.

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

Import this script through the RBAC custom role and then configure the users or groups that will have this role assigned.

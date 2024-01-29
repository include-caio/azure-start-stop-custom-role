## Custom role para ligar e desligar recursos no Azure

O objetivo dessa *custom role* é conceder o mínimo de permissões para automações que realizam a tarefa de ligar e desligar recursos no Azure

Para criar uma *custom role* é necessário possuir a permissão para executar a ação "Microsoft.Authorization/roleDefinitions/write", ação encontrada nas *roles* "Owner" e "User Access Administrator".\
Mais detalhes podem ser encontrados na [documentação oficial](https://learn.microsoft.com/en-us/azure/role-based-access-control/custom-roles)

## Como adicionar essa custom role?

- No escopo desejado, acesse o menu "Access control (IAM)", clique em "Add" e depois em "Add custom role"
<img src="https://i.imgur.com/w4c67dn.png" width="450">

- Selecione a opção "Start from JSON" e faça o upload do arquivo "custom-role.json" no campo "File"
<img src="https://i.imgur.com/aibUd4J.png" width="550">

- Edite as informações da aba "Assignable scope" adicionando o escopo desejado e removendo o que está lá
<img src="https://i.imgur.com/e6OnZ30.png" width="550">

- Após a criação, a *custom role* pode ser encontrada na aba "Roles". Para facilitar, o filtro "Type" pode ser alterado para "Custom" 
<img src="https://i.imgur.com/FlDU4iC.png" width="550">
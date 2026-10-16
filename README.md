# Mesa Pronta

Sistema de comandas para restaurantes: os atendentes lançam os pedidos pelo celular, a comanda sai na impressora térmica da cozinha e o dono gerencia cardápio, equipe e balanços. Tudo roda em um único computador dentro do restaurante, sem depender de internet.

Este repositório é a **vitrine pública** do Mesa Pronta. O código-fonte fica em um repositório privado; aqui ficam só os instaladores publicados em [Releases](../../releases).

## Instalador

Cada versão publica:

- `MesaPronta-Instalador-<versão>.exe`: instalador para Windows 10 ou 11 (64 bits);
- `versao.json`: número da versão, SHA-256 do instalador e novidades. O próprio Mesa Pronta consulta esse arquivo para avisar o administrador quando há uma versão nova.

O instalador não é assinado digitalmente; o Windows pode mostrar "Editor desconhecido". Antes de instalar, confira o SHA-256 no PowerShell:

```powershell
Get-FileHash .\MesaPronta-Instalador-<versão>.exe -Algorithm SHA256
```

O valor tem de ser igual ao publicado no release.

## Dados

Nenhum dado de restaurante, configuração real, certificado ou chave é publicado aqui. Cada instalação guarda os próprios dados no computador do restaurante.

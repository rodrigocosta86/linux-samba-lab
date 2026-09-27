# Linux Samba Lab

Laboratório prático de um servidor de arquivos Linux utilizando **Ubuntu Server e Samba**, criado para simular um ambiente empresarial com diferentes setores, usuários e níveis de acesso.

## 🎯 Objetivo

Construir um ambiente de laboratório para praticar administração de servidores Linux e compartilhamento de arquivos em rede.

O projeto simula três setores de uma empresa:

- Público
- Financeiro
- Administrativo

Cada setor possui regras próprias de acesso utilizando **usuários, grupos e permissões Linux/Samba**.

O laboratório também implementa recuperação de arquivos excluídos através do módulo `vfs_recycle` do Samba.

## 🛠️ Tecnologias utilizadas

- Ubuntu Server
- Samba
- Linux
- Windows
- VirtualBox
- SMB
- Cron

## 🏗️ Arquitetura

O ambiente foi estruturado da seguinte forma:

```text
        WINDOWS
           │
           │ SMB
           ▼
   UBUNTU SERVER
        SAMBA
           │
     /srv/samba/
           │
   ┌───────┼───────────┐
   ▼       ▼           ▼
Público  Financeiro  Administrativo
```

Os usuários recebem acesso aos compartilhamentos de acordo com os grupos aos quais pertencem.

## 🚧 Status

Laboratório funcional. Documentação e novas funcionalidades em evolução.

# 🚀✨ MINHA PRIMEIRA VM NO AZURE ✨🚀

> *Exercício Bootcamp Cloud Azure - DIO*

---

![Azure Badge](https://img.shields.io/badge/Azure-Cloud%20Bootcamp-blue) ![Status](https://img.shields.io/badge/Status–Conclu%C3%ADdo-brightgreen)

## 🎯 Objetivo

Criar uma Máquina Virtual (VM) no Microsoft Azure do zero, validando conceitos de IaaS e preparação de ambiente para próximos desafios do Bootcamp.

## 📋 Pré-requisitos

* Conta **Azure** ativa ✅
* Acesso ao **Portal** ou **Azure CLI** configurada 🔧
* Chave **SSH pública** (Linux) ou usuário/senha (Windows) 🔑

---

## 🛠️ Passo a Passo

1. **🔐 Login no Azure**

   * Acesse: [portal.azure.com](https://portal.azure.com)
   * Faça login com suas credenciais

2. **📦 Criar Resource Group**

   * Navegue em **Resource Groups** → **+ Create**
   * Defina:

     * **Nome:** `rg-bootcamp-vm`
     * **Região:** `Brazil South` (ou a de sua preferência)
   * Clique em **Review + create** → **Create**

3. **🖥️ Provisionar a VM**

   * Acesse **Virtual Machines** → **+ Create** → **Azure virtual machine**
   * Configure:

     * **Nome da VM:** `vm-bootcamp-dio`
     * **Image:** `Ubuntu 20.04 LTS`
     * **Size:** `Standard B1s`
     * **Autenticação:** **SSH public key**
     * **Usuário:** `azureuser`
     * **SSH key:** selecione sua chave existente

4. **🌐 Rede & Segurança**

   * **Virtual network:** `vnet-bootcamp`
   * **Subnet:** `default`
   * **Public IP:** `pip-vm-bootcamp`
   * **NSG:** padrão (porta **22** aberta para SSH)

5. **💾 Configurações de Disco**

   * **Tipo do disco OS:** `Standard SSD` (padrão)
   * **Monitoring:** desabilitado (para foco em deploy rápido)

6. **✅ Revisar & Criar**

   * Clique em **Review + create**
   * Confirme em **Create**
   * Aguarde (\~2 min) até a implantação finalizar

## 🚀 Próximos Passos

* Instalar linguagens e frameworks necessários (Node.js, Docker, etc.)
* Automatizar deploy com scripts
* Explorar serviços PaaS e IaC (ARM Templates/Terraform)

## 💡 Dica Final

> **Economize custos!**
> Após os testes, delete o **Resource Group** `rg-bootcamp-vm` para não gerar cobranças indesejadas.

---

*🗓️ 17 de maio de 2025 — Bootcamp Cloud Azure | DIO*

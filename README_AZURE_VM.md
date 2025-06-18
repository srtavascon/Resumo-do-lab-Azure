
# 💻 Azure Virtual Machines – Criação e Gerenciamento de uma VM Windows

Este guia tem como objetivo consolidar o conhecimento sobre **criação, acesso, configuração e exclusão de máquinas virtuais (VMs)** no **Microsoft Azure**, utilizando o **Portal Web** para criação de uma VM com **Windows Server 2022 Datacenter**.

---

## ✅ Aplica-se a:
- Máquinas Virtuais (VMs) com Windows

As VMs do Azure podem ser criadas diretamente pelo **Portal do Azure**, oferecendo uma interface gráfica para criação e gerenciamento.

---

## 🧱 1. Criar uma Máquina Virtual

### Passos:

1. No Portal do Azure, digite `Máquinas virtuais` na barra de pesquisa.
2. Em **Serviços**, selecione **Máquinas virtuais**.
3. Na página **Máquinas virtuais**, clique em **Criar** > **Máquina virtual do Azure**.
4. Na seção **Detalhes da instância**:
   - Nome da VM: `myVM`
   - Imagem: `Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2`
   - Conta de administrador:
     - Nome de usuário: ex. `azureuser`
     - Senha: mínimo de 12 caracteres com complexidade
5. Em **Regras de porta de entrada**, selecione:
   - Permitir portas selecionadas: `RDP (3389)` e `HTTP (80)`
6. Clique em **Examinar + criar**, depois em **Criar**.
7. Após a conclusão, clique em **Ir para o recurso**.

---

## 🔐 2. Conectar-se à VM via RDP

1. Na página da VM, clique em `Conectar > RDP`.
2. Na aba **Conectar-se ao RDP**, mantenha as opções padrão (endereço IP e porta 3389).
3. Clique em **Baixar arquivo RDP**.
4. Abra o arquivo `.rdp` baixado e clique em **Conectar**.
5. Quando solicitado:
   - Clique em **Mais opções > Usar uma conta diferente**
   - Digite: `localhost\nome-de-usuário`
   - Insira a senha criada na etapa anterior
6. Se aparecer um aviso de certificado, clique em **Sim** ou **Continuar**.

---

## 🌐 3. Instalar o Servidor Web (IIS)

Para verificar o funcionamento da VM:

1. Conecte-se à VM via RDP
2. Abra o PowerShell como Administrador
3. Execute o comando:

```powershell
Install-WindowsFeature -name Web-Server -IncludeManagementTools
```

4. Quando terminar, feche a conexão RDP com a VM.

---

## 📴 4. Configurar Desligamento Automático

1. Na página da VM, vá em **Operações > Desligamento automático**
2. Clique em **Ativado**
3. Defina o **horário desejado**
4. Configure o **fuso horário** corretamente (padrão: UTC)
5. Clique em **Salvar**

---

## 🧹 5. Excluir Recursos

Para evitar custos adicionais:

1. Na página da VM, clique no link **Grupo de Recursos**
2. Clique em **Excluir grupo de recursos**
3. Digite o nome do grupo e confirme

---

## 📌 Observações Finais

- ✅ Ideal para testes e labs com Windows Server
- 🔐 Habilite somente as portas necessárias (segurança)
- 💰 Use desligamento automático e exclua recursos quando não estiverem em uso

---

**Tags**: `Azure` `Máquinas Virtuais` `Windows Server` `Portal do Azure` `Cloud`

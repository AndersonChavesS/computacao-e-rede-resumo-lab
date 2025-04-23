## Bootcamp Java Cloud Native - Bradesco | DIO
###  Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure
Este repositório contém um resumo da aula sobre **Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure**, abordando os principais conceitos de computação e rede no Microsoft Azure. A seguir, você encontrará um guia prático sobre como criar e configurar uma máquina virtual no Azure, além de tópicos relacionados à otimização de recursos.

---

## Sumário

1. [Assinatura de Plataforma MSDN](#assinatura-de-plataforma-msdn)
2. [Criando uma Máquina Virtual no Azure](#criando-uma-máquina-virtual-no-azure)
3. [Configuração de Escala e Condição de Escala](#configuração-de-escala-e-condição-de-escala)
4. [Selecionar um Tamanho de VM](#selecionar-um-tamanho-de-vm)
5. [Ligamento/Desligamento Automático da VM](#ligamentodesligamento-automático-da-vm)
6. [Habilitação de Backup](#habilitação-de-backup)
7. [Configurar Regras de Alerta Recomendada](#configurar-regras-de-alerta-recomendada)
8. [Área de Trabalho Virtual do Azure](#área-de-trabalho-virtual-do-azure)
9. [Criar Aplicativo de Funções](#criar-aplicativo-de-funções)

---

## Assinatura de Plataforma MSDN

A **Assinatura MSDN** é uma oferta especial para desenvolvedores que fornece créditos mensais no Azure, permitindo explorar e testar serviços sem custos adicionais. Esses créditos podem ser usados para criar máquinas virtuais, configurar redes e experimentar outros recursos do Azure.

Para acessar:
1. Entre no portal do Azure com sua conta MSDN.
2. Verifique seus créditos disponíveis na seção "Benefícios do Azure".

---

## Criando uma Máquina Virtual no Azure

Passo a passo para criar uma máquina virtual no Azure:

1. **Acessar o Portal do Azure**:
   - Entre no [portal do Azure](https://portal.azure.com).

2. **Criar uma Máquina Virtual**:
   - Clique em **Criar um recurso**.
   - Selecione **Máquina Virtual**.

3. **Configurações Básicas**:
   - Escolha uma assinatura (MSDN ou outra disponível).
   - Defina um grupo de recursos ou crie um novo.
   - Nomeie a máquina virtual.
   - Selecione a região desejada.

4. **Imagem e Autenticação**:
   - Escolha uma imagem de sistema operacional (ex.: Ubuntu, Windows Server).
   - Configure autenticação por senha ou chave SSH.

5. **Rede**:
   - Configure uma nova ou use uma rede virtual existente.
   - Defina as portas de entrada (ex.: HTTP, HTTPS, SSH).

6. **Revisão e Criação**:
   - Revise todas as configurações.
   - Clique em **Criar** para provisionar a VM.

---

## Configuração de Escala e Condição de Escala

O Azure permite dimensionar automaticamente suas máquinas virtuais com base em condições específicas, como carga de CPU ou memória.

### Passos:
1. Acesse a VM no portal do Azure.
2. Vá para **Dimensionamento automático**.
3. Configure uma **Condição de Escala**:
   - Exemplo: Aumentar o número de instâncias quando a CPU ultrapassar 80%.
4. Salve as alterações.

---

## Selecionar um Tamanho de VM

O tamanho da VM define os recursos de computação (CPU, memória, disco) disponíveis.

### Como escolher:
1. Durante a criação da VM, selecione **Tamanho**.
2. Escolha um tamanho com base nas necessidades:
   - **Pequeno**: Para testes ou desenvolvimento.
   - **Grande**: Para cargas de trabalho intensas.

---

## Ligamento/Desligamento Automático da VM

Você pode automatizar o ligamento e desligamento da VM para economizar custos.

### Configuração:
1. No portal do Azure, vá para **Automação de Processos**.
2. Crie uma **Regra de Agendamento**:
   - Defina horários para ligar/desligar a VM.

---

## Habilitação de Backup

O backup garante que seus dados estejam protegidos.

### Como habilitar:
1. Acesse a VM.
2. Vá para **Backup**.
3. Configure o cofre de serviços de recuperação.
4. Defina a frequência do backup.

---

## Configurar Regras de Alerta Recomendada

Alertas ajudam a monitorar o desempenho da VM.

### Configuração:
1. Vá para **Monitoramento > Alertas**.
2. Crie uma nova regra:
   - Exemplo: Receber notificação se a CPU ultrapassar 80%.

---

## Área de Trabalho Virtual do Azure

A Área de Trabalho Virtual do Azure permite acessar ambientes Windows diretamente do navegador.

### Como configurar:
1. No portal do Azure, procure por **Área de Trabalho Virtual do Windows**.
2. Crie um pool de hosts e configure as máquinas virtuais associadas.

---

## Criar Aplicativo de Funções

Os aplicativos de funções permitem executar código sem gerenciar infraestrutura.

### Passos:
1. No portal do Azure, clique em **Criar um recurso**.
2. Selecione **Aplicativo de Funções**.
3. Configure as opções básicas (assinatura, grupo de recursos, etc.).
4. Escolha o runtime (.NET, Node.js, etc.).
5. Publique suas funções via portal ou CLI.

---

## Conclusão

Este guia apresentou os principais passos para configurar e gerenciar máquinas virtuais no Azure, desde a criação até a otimização de recursos. Com essas práticas, você estará preparado para implementar soluções eficientes e escaláveis na nuvem.

---

**Referências**:
- [Documentação Oficial do Azure](https://docs.microsoft.com/pt-br/azure/)
- Bootcamp Java Cloud Native - Bradesco | DIO

**Guia Completo do Ciclo de Vida de Documentos no Sistema de Gestão**

---

## **✍️ Objetivo**

Este documento tem como objetivo detalhar de forma clara, dinâmica e acessível o fluxo completo de gestão de documentos no sistema utilizado, com orientações tanto para usuários comuns quanto para administradores. A proposta é garantir rastreabilidade, conformidade e segurança documental.

---

## **🔄 Visão Geral do Fluxo Documental**

1. **Elaboração**  
2. **Revisão**  
3. **Aprovação**  
4. **Publicação / Documento Aprovado**  
5. **Obsolescência**

Cada fase é composta por campos obrigatórios, ações automatizadas e permissões diferenciadas por perfil.

---

## **✏️ 1\. Elaboração**

### **Descrição**

Esta é a etapa inicial de criação do documento. O responsável pela elaboração é quem inicia o ciclo.

### **Ações:**

* Preencher os campos obrigatórios: Título, Tipo, Descrição e Responsável, .  
* Criar o conteúdo do documento (pode estar em anexo ou texto no sistema).  
* Acionar o botão **"Enviar para Análise"**.

### **Campos Visíveis:**

* ID  
* Doc. Pai  
* Nome do documento  
* Versão  
* Tipo  
* Descrição  
* Responsável  
* Aprovador/Revisor  
* Anexo  
* Botão de Envio para análise  
* Excluir

### **Permissões:**

* Apenas o **elaborador** pode editar.

---

## **🖊️ 2\. Revisão**

### **Descrição**

Após a validação do aprovador, caso necessário, o documento é encaminhado para revisão técnica. Um revisor designado (responsável pelo documento ou não) ajusta o que foi solicitado pelo aprovador.

### **Ações:**

* Validar coerência e conformidade do conteúdo.  
* Através do botão **"Enviar para Aprovação"**, encaminhar para próxima etapa (nova análise).

### **Campos Visíveis:**

* ID  
* Doc. Pai  
* Título do Documento  
* Versão atual  
* Descrição  
* Responsável  
* Anexo  
* Aprovador/Revisor  
* Obs. do Aprovador  
* Enviar para análise

### **Permissões:**

* Apenas o **revisor/elaborador** pode editar nesta etapa.

---

## **📄 3\. Aprovação**

### **Descrição**

O aprovador analisa o documento elaborado/revisado e decide pela sua aprovação final.

### **Ações:**

* Conferir todas as informações.  
* Se aprovado: clicar em **"Aprovar"**.  
* Se reprovado: clicar em **"Reprovar e Devolver"** para a revisão.

### **Campos Editáveis:**

* Correções/Alterações a fazer

### **Permissões:**

* Apenas o **aprovador** tem controle nesta etapa.

---

## **📅 4\. Documento Aprovado**

### **Descrição**

Após a aprovação, o documento é considerado vigente e ativo. Aparece em listas e relatórios.

### **Ações:**

* Distribuição interna (manual ou automatizada)  
* Armazenamento adequado no repositório do sistema

### **Campos Visíveis:**

* Diretoria  
* Tipo  
* ID  
* Título do doc  
* Versão atual  
* Detalhes do documento  
* Prazos do documento  
* Indicador de prazo  
* Responsável atribuído  
* Docs anexados  
* Aprovador/Revisor  
* Data de aprovação  
* Alterar  
* Arquivar  
* Renovar doc.  
* Motivo do Bloqueio

### **Permissões:**

* **Leitura para todos os colaboradores**.  
* Apenas **administradores/elaboradores** podem arquivar ou substituir versão.

---

## **📁 5\. Obsolescência**

### **Descrição**

Quando o documento perde validade (por revisão, vencimento ou substituição), ele é movido para a lista de obsoletos.

### **Ações:**

* Clicar em **"Arquivar "** (somente administradores e aprovadores/elaboradores).  
* O documento permanece registrado no histórico.

### **Campos Visíveis:**

* ID  
* Título do doc  
* Tipo  
* Versão atual  
* Detalhes do documento  
* Responsável atribuído  
* Prazos do documento  
* Docs anexados  
* Aprovador/Revisor  
* Data de aprovação  
* Obs. do Aprovador/Revisor  
* Renovar doc.  
* Motivo do bloqueio

### **Permissões:**

* Apenas **administradores** podem mover documentos para obsoletos.

---

## **📆 Campos Padrão do Sistema**

| Título do documento | Tipo | Obrigatório | Nome descritivo |
| :---- | :---- | :---- | :---- |
| Tipo de documento | Lista | Sim | Política, Procedimento, Instrução etc |
| Setor | Lista | Sim | Diretoria ou área responsável |
| Responsável | Pessoa | Sim | Autor ou elaborador principal |
| Versão | Texto | Sim | Ex: v1.0, v2.1 |
| Anexo | Arquivo | Opcional | PDF, DOCX, etc |

---

## **🧬 Perfis e Permissões**

| Perfil | Permissões |
| :---- | :---- |
| Usuário comum | Visualiza documentos aprovados |
| Revisor | Visualiza \+ revisa documentos enviados |
| Aprovador | Aprova ou reprova documentos em revisão |
| Admin | Controla status, arquiva, edita qualquer documento |
| Elaborador | Elabora e revisa documentos |

---

## **🔧 Funcionalidades Dinâmicas no Coda**

* **Botões personalizados**: Enviar para revisão, Aprovar, Arquivar.  
* **Views filtradas**: Documentos em elaboração, aprovados, obsoletos.  
* **Automatizações**: E-mails automáticos, data de vencimento, logs de versão.  
* **Controle de versão**: Registro histórico com versões anteriores e autorias.

---

## **ℹ️ Suporte**

Em caso de dúvidas ou problemas com o sistema de documentos, entre em contato com cssbreno.dev@gmail.com.

---

**Versão do Guia:** 1.0

**Data de publicação:** 05/05/2025

**Responsável:** Equipe de Gestão Documental


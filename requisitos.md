# Requisitos – Comparacao_Minuta_vs_Dados

## Regras de Negócio

### **1. Regras de Seleção**
- Apenas itens marcados como aptos devem ser considerados para execução.
- Em caso de ausência de itens, registrar execução sem processamento.

### **2. Regras para Captura de Dados**
- Sempre validar se o nome do comprador corresponde ao nome do documento.
- Identificar corretamente comprador adicional quando existir.
- Capturar informações do empreendimento completas.

### **3. Regras de Preenchimento**
- Planilhas devem ser preenchidas conforme modelo padrão.
- Dados da minuta devem ser substituídos integralmente conforme parágrafos mapeados.
- Campos financeiros devem sempre ser comparados com os valores capturados.

### **4. Regras para Emissão de Documentos**
- ITBI só deve ser emitido se valor de compra e venda estiver dentro do limite definido.
- Declaração de Isenção é gerada apenas quando aplicável.
- Documento de 1ª Aquisição deve refletir corretamente se é primeira ou segunda aquisição.

### **5. Regras de Consolidação**
- Todos os documentos devem ser consolidados em PDF único.
- A nomenclatura do arquivo deve seguir obrigatoriamente o padrão:
- DDMMYY_Comprador_CPF_Bloco_Unidade

### **6. Regras de Assinatura**
- Ordem da fila deve respeitar a planilha auxiliar.
- O procurador deve ser sempre o último aprovador.

---

## 🔍 Validações Necessárias
- Verificar existência dos documentos auxiliares.
- Validar estrutura e layout dos arquivos antes de editar.
- Comparar valores financeiros:
- Financiamento
- FGTS
- Subsídio
- Recursos Próprios
- Verificar presença dos parágrafos obrigatórios.
- Validar campos obrigatórios:
- Fração 
- Matrícula
- Cartório
- Data
- Certificar que documentos complementares foram gerados.
- Validar que o PDF final contém todas as partes.

---

## 📤 Saídas Esperadas
- Minuta final editada e padronizada.
- Documentos auxiliares preenchidos:
- Declaração para Isenção (quando aplicável)
- Documento de 1ª Aquisição (quando aplicável)
- Ficha e Guia do ITBI (quando aplicável)
- Arquivo PDF consolidado final.
- Fila estruturada para assinatura.
- Relatório analítico contendo:
- Capturas
- Divergências
- Exceções
- Relatório sintético consolidado.

---

## 🏆 Critérios de Sucesso
- Documento final gerado sem divergências.
- Todos os parágrafos substituídos corretamente.
- Assinaturas configuradas conforme ordem definida.
- ITBI emitido somente quando aplicável.
- Planilhas auxiliares preenchidas integralmente.
- Nenhuma quebra de fluxo por falta de dados.
- Tempo total de execução reduzido em relação ao processo manual.
- Logs claros e todas as exceções registradas corretamente.


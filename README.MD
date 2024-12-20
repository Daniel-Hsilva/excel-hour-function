
# Função de Cálculo de Horas no Excel

## 📝 Descrição
Este projeto contém uma fórmula personalizada criada no Excel para calcular a diferença entre datas e horas, considerando cenários específicos como intervalos ou diferentes formatos de entrada.

A fórmula foi desenvolvida com a função **LAMBDA & LET** do Excel, permitindo reutilização eficiente sem a necessidade de código VBA.

---

## 🚀 Funcionalidades
- Calcula a diferença entre datas e horas.
- Ajusta automaticamente os formatos de entrada das horas.
- Retorna um valor personalizado quando os dados estão incompletos.
- Fácil de integrar em planilhas existentes.

---

## 📦 Estrutura dos Arquivos
- **`calculo_horas.xlsx`**: Planilha de exemplo contendo a fórmula funcional e casos de teste.
- **`calculo_horas.txt`**: Texto contendo apenas a fórmula para uso rápido.
- **`README.md`**: Este arquivo, explicando o projeto.

---

## 🛠️ Como Usar
1. **Importe a Fórmula na Planilha:**
   - Copie a fórmula do arquivo `calculo_horas.txt` ou abra a planilha `calculo_horas.xlsx`.

2. **Configuração da Fórmula:**
   A fórmula é utilizada no seguinte formato:
   
   =HORAS.TOTAIS(data_inicial; data_final; hora_inicial; hora_final; [se_vazio]; ...)
   
   - **`data_inicial`**: Data de início (obrigatório).
   - **`data_final`**: Data final (obrigatório).
   - **`hora_inicial`**: Hora de início no formato `hh:mm` ou `hhmm` (obrigatório).
   - **`hora_final`**: Hora final no formato `hh:mm` ou `hhmm` (obrigatório).
   - **`[se_vazio]`**: Valor retornado se algum campo estiver vazio (opcional).

3. **Exemplo de Uso:**
   Suponha que as células contenham os seguintes valores:
   - `A1`: `01/12/2024` (data inicial).
   - `B1`: `02/12/2024` (data final).
   - `C1`: `0800` (hora inicial).
   - `D1`: `1730` (hora final).

   A fórmula seria:
   
   =HORAS.TOTAIS(A1; B1; C1; D1; "Dados insuficientes")
   

---

## ✅ Pré-requisitos
- **Microsoft Excel 365**: Suporte para a função `LAMBDA`.
- Conhecimento básico em fórmulas do Excel.

---

## 📂 Exemplos de Resultados
| Data Inicial | Data Final   | Hora Inicial | Hora Final | Resultado   |
|--------------|--------------|--------------|------------|-------------|
| 01/12/2024   | 01/12/2024   | 08:00        | 17:30      | 9:30        |
| 01/12/2024   | 02/12/2024   | 22:00        | 06:00      | 8:00        |
| 01/12/2024   | (vazio)      | 08:00        | 17:30      | Dados insuficientes |

---

## ✨ Contribuições
Sinta-se à vontade para sugerir melhorias ou reportar problemas no [repositório GitHub](https://github.com/Daniel-Hsilva).

---

## 🖥️ Autor
Desenvolvido por [Daniel Henrique](www.linkedin.com/in/danielhsilva44).
Compartilhe seu feedback e ideias para aprimorar este projeto! 🚀

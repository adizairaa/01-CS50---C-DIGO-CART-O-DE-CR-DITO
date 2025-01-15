### Descrição para o Repositório do GitHub

---

# 💳 Validação de Cartões de Crédito  

Este repositório contém uma implementação em C para validar números de cartões de crédito utilizando o **Algoritmo de Luhn**. O programa determina se um número é válido e identifica a bandeira do cartão (AMEX, MASTERCARD ou VISA) com base em seus padrões.

---

## 🧠 **Contexto**  

Os números dos cartões de crédito seguem regras específicas:  
- **American Express (AMEX)**: 15 dígitos, começando com 34 ou 37.  
- **MasterCard**: 16 dígitos, começando com 51, 52, 53, 54 ou 55.  
- **Visa**: 13 ou 16 dígitos, começando com 4.  

Além disso, utilizam o **Algoritmo de Luhn** para verificar erros de digitação ou números inválidos.  

---

## ⚙️ **Como o Programa Funciona**  

1. **Entrada do Usuário:**  
   O usuário insere um número de cartão sem espaços ou traços.  

2. **Validação do Comprimento e Prefixo:**  
   - O comprimento e os dígitos iniciais do número são usados para determinar a possível bandeira do cartão.  

3. **Aplicação do Algoritmo de Luhn:**  
   - Multiplicamos cada segundo dígito, a partir do penúltimo, por 2.  
   - Somamos os dígitos resultantes ao restante dos dígitos.  
   - Validamos se o total é múltiplo de 10.  

4. **Saída:**  
   - O programa retorna a bandeira do cartão (AMEX, MASTERCARD ou VISA) ou indica que o número é inválido.  

---

## 📂 **Estrutura do Código**  

- **Arquivo principal:** `credit.c`  
- **Funções principais:**  
  - `checksum`: Implementa o Algoritmo de Luhn.  
  - `main`: Gerencia a entrada, valida o número e imprime o resultado.  

---

## 🚀 **Como Usar**  

1. Clone este repositório:  
   ```bash
   git clone https://github.com/seuusuario/validacao-cartao.git
   cd validacao-cartao
   ```

2. Compile o código:  
   ```bash
   make credit
   ```

3. Execute o programa:  
   ```bash
   ./credit
   ```

4. Insira um número de cartão quando solicitado.

---

## ✅ **Exemplo de Entrada e Saída**  

### Entrada:  
```bash
Número: 4003600000000014
```

### Saída:  
```bash
VISA
```

---

## 🛠️ **Ferramentas e Testes**  

- **CS50 Library:** Utilizada para facilitar o input de números longos.  
- **check50:** Validação automatizada da solução.  
- **style50:** Garantia de estilo de código limpo e legível.  

---

## 🌟 **Contribuições**  

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests para melhorias ou novos recursos.  

---

## 📜 **Licença**  

Este projeto está licenciado sob a [MIT License](LICENSE).  

--- 

Se precisar de mais informações ou ajustes, é só pedir! 😊

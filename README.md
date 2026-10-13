# Assinaturas Oficiais — CSC Veneza Equipamentos

Repositório público de assets estáticos do Centro de Soluções Conectadas (CSC) da Veneza Equipamentos.
Hospeda as assinaturas visuais dos operadores de regional para uso no Envio Mensal de Relatórios RDA via automação n8n.

## Operadores e Regionais

| Regional | Operador | Base | Imagem Direta | Página Individual |
| :--- | :--- | :--- | :--- | :--- |
| **R1** | Oscar Rabelo | Recife / PE | `oscar.jpg` | [r1.html](r1.html) |
| **R2** | Eduardo Souza | Bahia / BA | `eduardo.jpg` | [r2.html](r2.html) |
| **R3** | Luis Jucá | Fortaleza / CE | `luis.jpg` | [r3.html](r3.html) |

## Como utilizar no n8n (RDA Envio Mensal)

No nó `Preparar Lista de Clientes` (ou equivalente de montagem do HTML do e-mail):

```javascript
const URL_BASE = 'https://jhonataleoncio.github.io/assinaturas-regionais-csc';

const ASSINATURAS = {
  R1: `${URL_BASE}/oscar.jpg`,
  R2: `${URL_BASE}/eduardo.jpg`,
  R3: `${URL_BASE}/luis.jpg`
};
```

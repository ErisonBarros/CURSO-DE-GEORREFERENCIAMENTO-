---
icon: wagon-covered
---

# PRECISÃO E EXATIDÃO

#### 🧠 **1. Conceitos Fundamentais**

*   **Exatidão (Accuracy)**\
    Representa o **grau de conformidade** entre o valor medido e o valor verdadeiro.

    > Exatidão = quão **próxima** a medida está do valor real.
*   **Precisão (Precision)**\
    Representa o **grau de repetibilidade** ou consistência das medições.

    > Precisão = quão **consistentes** são os resultados entre si, mesmo que estejam longe do valor real.

***

#### 📊 **2. Diferença entre Precisão e Exatidão**

| Medidas                        | Exatidão | Precisão | Explicação                              |
| ------------------------------ | -------- | -------- | --------------------------------------- |
| Alta exatidão, alta precisão   | ✅        | ✅        | Valores concentrados próximos do real   |
| Alta exatidão, baixa precisão  | ✅        | ❌        | Médias corretas, mas dispersas          |
| Baixa exatidão, alta precisão  | ❌        | ✅        | Resultados agrupados, mas longe do real |
| Baixa exatidão, baixa precisão | ❌        | ❌        | Resultados dispersos e longe do real    |

***

#### 🎯 **3. Figuras Explicativas**

Vamos usar o clássico exemplo de um **alvo de tiro ao alvo** para representar os conceitos:

**✅ Exatidão e Precisão Alta:**

![Alvo com tiros agrupados no centro (alta precisão e alta exatidão)](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Accuracy_and_precision.svg/800px-Accuracy_and_precision.svg.png)

**❌ Alta Precisão, Baixa Exatidão:**

Tiros agrupados, mas longe do centro (valor real).

**❌ Alta Exatidão, Baixa Precisão:**

Tiros espalhados, mas em média próximos do centro.

**❌ Baixa Exatidão e Baixa Precisão:**

Tiros dispersos e longe do centro.

#### 🧪 **4. Aplicações Práticas em Geociências**

* Em **GNSS**, um receptor pode ter:
  * Alta **precisão** nos pontos (repetibilidade do ponto),
  * Mas **baixa exatidão** se houver erro sistemático (offset).
* Em **levantamentos topográficos**, medições repetidas com:
  * Pequena dispersão → alta **precisão**,
  * Correção com referência conhecida → aumenta a **exatidão**.

***

#### 🧩 **5. Atividade Prática**

**Simulação com medições de distância (exemplo com trena ou estação total):**

```plaintext
Valor verdadeiro: 50,000 m

Medições do Grupo A: 49,998 / 49,997 / 49,996
→ Alta precisão, baixa exatidão

Medições do Grupo B: 50,002 / 49,998 / 50,001
→ Alta exatidão, baixa precisã
```

***

#### 📌 **6. Resumo Visual Final**

```markdown
🎯 Exatidão → Aproximação do valor real  
🎯 Precisão → Repetibilidade entre medições  
✔️ Ideal: alta precisão e alta exatidão  
⚠️ Cuidado: nem sempre medições agrupadas são corretas!
```

***

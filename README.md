# Habit Tracker Pro

Rastreador de hábitos pessoal, simples e direto. Tudo funciona no navegador — sem cadastro, sem servidor, sem nuvem. Os dados ficam salvos localmente no seu dispositivo.

🌐 **Acesse em:** [habittracker.zava.dev.br](https://habittracker.zava.dev.br)

---

## Como funciona

### Abas de frequência

O tracker é dividido em abas conforme a frequência dos seus hábitos:

| Aba | Uso |
|---|---|
| **Diário** | Hábitos que devem ser feitos todos os dias |
| **Comercial** | Tarefas do dia útil (prospecção, CRM, redes sociais…) |
| **Autocuidado** | Rotinas de beleza e saúde, organizadas em categorias |
| **Saúde** | Remédios, suplementos e medicamentos |
| **Semanal** | Tarefas que bastam ser feitas uma vez por semana |
| **Mensal** | Compromissos mensais (contas, consultas, manutenção…) |
| **Anual** | Mapa de calor com a sua consistência ao longo do ano |

---

### Marcando um hábito

Clique no quadrado correspondente ao dia para alternar entre três estados:

| Estado | Visual | Significado |
|---|---|---|
| *(vazio)* | Borda cinza | Ainda não feito |
| **✓** | Verde | Feito |
| **–** | Cinza escuro | Não aplicável / pulado |
| **✕** | Vermelho claro | Não feito (dia já passou) |

> Hábitos **semanais** e de **autocuidado** ficam automaticamente marcados como "–" nos outros dias da semana assim que você marcar um deles como feito.

---

### Navegação por semana

Use as setas **← →** no canto superior direito para navegar entre semanas e visualizar o histórico. O botão **HOJE** retorna à semana atual.

Você também pode clicar diretamente na **data** no topo para ir a qualquer semana específica.

---

### Gerenciando hábitos

#### Adicionar um hábito

1. Selecione a aba desejada
2. Clique em **+ Novo Hábito**
3. Se a aba tiver categorias, escolha em qual delas o hábito entrará (ou deixe "Sem categoria")
4. Digite o nome e confirme

#### Adicionar uma categoria

Categorias agrupam hábitos dentro de uma aba (como "Cabelo", "Skincare", "Pós Banho" dentro de Autocuidado).

1. Selecione a aba desejada
2. Clique em **+ Nova Categoria**
3. Digite o nome e confirme

#### Reordenar

Passe o mouse sobre um hábito ou categoria para revelar os botões **▲ ▼** e arraste-o para cima ou para baixo na lista.

#### Remover um hábito ou categoria

Passe o mouse sobre o item e clique no **✕** que aparece à direita.

A remoção é **não-destrutiva**: o hábito some das semanas futuras, mas o histórico passado é preservado. Você continua vendo os registros anteriores ao navegar para semanas passadas.

---

### Backup e restauração

Seus dados ficam no `localStorage` do navegador. Para não perder nada ao trocar de dispositivo ou limpar o browser:

- **Backup** — exporta um arquivo `.json` com todo o seu histórico
- **Restaurar** — importa um arquivo `.json` exportado anteriormente

> Faça backup regularmente se usar o tracker no celular, pois browsers móveis limpam o `localStorage` com mais frequência.

---

### Mapa de calor anual

A aba **Anual** exibe um heatmap mês a mês mostrando quantos hábitos diários você completou em cada dia do ano. Útil para identificar padrões e semanas de baixa consistência.

Use as setas **← →** dentro da aba para navegar entre anos.

---

## Tecnologia

- HTML + CSS + JavaScript puro — sem dependências de backend
- [Tailwind CSS](https://tailwindcss.com) via CDN para estilização
- `localStorage` para persistência dos dados
- Hospedado via GitHub Pages

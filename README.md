# Monitoramento Simulado de Atuador Industrial

Projeto de estudo que simula um sistema de monitoramento industrial, aplicando os fundamentos de módulos em Python para gerar e registrar dados de sensores.

## O que foi estudado

| Módulo | Aplicação no projeto |
|--------|----------------------|
| `math` | Cálculo da circunferência da engrenagem a partir do diâmetro (`math.pi`) |
| `random` | Geração de leituras simuladas — posição (`uniform`) e temperatura (`randint`) |
| `datetime` | Registro de data e hora de cada evento de monitoramento (`strftime`) |

## Estrutura do código

- **Constantes** — Define o diâmetro da engrenagem (50 mm) e calcula a circunferência.
- **`simular_leitura_sensor()`** — Retorna valores aleatórios de posição (0–100%) e temperatura (25–80 °C).
- **`registrar_evento()`** — Formata e imprime um log com timestamp, posição e temperatura.
- **Laço principal** — Executa 5 ciclos de monitoramento, chamando as funções acima.

## Como executar

```bash
python main.py
```

## Exemplo de saída

```
--- Iniciando Monitoramento Simulado de Atuador Industrial ---
Configuração: Circunferência da Engrenagem = 157.08 mm
------------------------------------------------------------
[2025-07-15 14:30:01] LOG ATUADOR: Posição=72.45%, Temp=53°C
[2025-07-15 14:30:01] LOG ATUADOR: Posição=14.89%, Temp=67°C
[2025-07-15 14:30:01] LOG ATUADOR: Posição=91.03%, Temp=29°C
[2025-07-15 14:30:01] LOG ATUADOR: Posição=46.72%, Temp=74°C
[2025-07-15 14:30:01] LOG ATUADOR: Posição=8.31%, Temp=41°C
------------------------------------------------------------
--- Fim do Monitoramento ---
```

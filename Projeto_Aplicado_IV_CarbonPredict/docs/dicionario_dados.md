# Dicionário de Dados — CarbonPredict

## Variáveis previstas da base integrada

| Variável | Tipo | Unidade/Formato | Origem | Descrição |
|---|---|---|---|---|
| `data` | data | AAAA-MM | EPE/IBGE/MCTI | Competência temporal |
| `regiao` | categórica | texto | EPE | Região geográfica |
| `setor_industrial` | categórica | texto/código | EPE | Setor industrial CNAE 2.0 |
| `consumo_mwh` | numérica | MWh | EPE | Consumo mensal de energia elétrica |
| `indice_producao` | numérica | índice | IBGE/PIM-PF | Indicador de produção física industrial |
| `fator_emissao_tco2_mwh` | numérica | tCO₂/MWh | MCTI/SIRENE | Fator médio de emissão associado à eletricidade |
| `emissao_estimada_tco2` | numérica | tCO₂ | Derivada | Consumo × fator de emissão |
| `lag_1` | numérica | MWh | Derivada | Consumo do mês anterior |
| `lag_12` | numérica | MWh | Derivada | Consumo do mesmo mês do ano anterior |
| `media_movel` | numérica | MWh | Derivada | Média móvel a definir na modelagem |
| `mes` | inteira | 1–12 | Derivada | Mês da observação |
| `trimestre` | inteira | 1–4 | Derivada | Trimestre da observação |

> O dicionário será atualizado após a inspeção dos arquivos brutos e a confirmação dos nomes e tipos originais das colunas.

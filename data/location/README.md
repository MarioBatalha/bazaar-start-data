# Bazaar API - Location Start Data

Alguns dados no bazaar precisam ser pre criados e injectados ( como as categorias do bazaar ) afim de dar suporte a outras extruturas automática.

Daí, este pequeno repositório, onde poderás contribuir adicionando mais dados ou usar os dados já cadastrados para o que desejares.

---------------------------------------------

## Dados de Localizacao do Bazaar

As localizacoes do bazaar têm uma extrutura base muito simples: `Pais -> Provincia -> Municipio -> Distrito`

```json
    [
        // Paises
        {
            "name": "Angola",
            "provinces": [
                {
                    "name": "Luanda",
                    "counties": [
                        {
                            "name": "Belas",
                            "districts": [
                                {
                                    "name": "Kilamba"
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    ]
```
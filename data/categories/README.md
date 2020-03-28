# Bazaar API - Categories Start Data

Alguns dados no bazaar precisam ser pre criados e injectados ( como as categorias do bazaar ) afim de dar suporte a outras extruturas automática.

Daí, este pequeno repositório, onde poderás contribuir adicionando mais dados ou usar os dados já cadastrados para o que desejares.

---------------------------------------------

## Dados de Categorias do Bazaar

As categorias do bazaar têm uma extrutura base muito simples: `MasterCategory -> Category -> SubCategory`

```json
    [
        // MasterCategory
        {
            "name": "Tecnologia",
            "hex_color": "#0078D7",
            "fa_icon": "<i class='fas fa-laptop'></i>",
            "subcategories": [
                // Category
                {
                    "name": "Computadores",
                    "subcategories": [
                        // SubCategory
                        {
                            "name": "Componentes",
                            "tags": "memoria ram, rom, hd, placa grafica, disco duro",
                            // datalhes => <Tipo de Dados:Nome> ;
                            "details_keys": "<bool:Usado>;<str:Marca>;<:>"
                        }
                    ]
                }
            ]
        },
        {
            "name": "Outros",
            "subcategories": [
                {
                    "name": "Outros",
                    "subcategories": [
                        {
                            "name": "Outros"
                        }
                    ]
                }
            ]
        }
    ]
```

### Tipos de Dados em Datalhes `<tipo:nome>;`

Tipos de dados

- `str` Para (String) cadeia de caracteres incluindo digitos
- `bool` Para (Boolean) sim ou não
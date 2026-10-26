# StockGuard – Práctica de GitHub Actions

Proyecto de práctica para la Línea de Profundización I – Big Data
(Universidad de Cundinamarca, Extensión Facatativá).

## Qué hace
Clasifica el nivel de riesgo del inventario de un producto según el stock
actual y el stock mínimo: AGOTADO, CRITICO, BAJO o NORMAL. También detecta
sobrestock con `detectar_sobrestock`.

## Estructura
- `src/inventario.py`: reglas de negocio.
- `tests/test_inventario.py`: pruebas con pytest.
- `.github/workflows/ci.yml`: workflow de GitHub Actions.

## Cómo ejecutar las pruebas
    python -m pip install -r requirements.txt
    python -m pytest -v

## Integración continua
El workflow "CI StockGuard" se ejecuta en cada push o Pull Request hacia
`main`, y también de forma manual. Valida la sintaxis y corre las pruebas.

Autora: Laura Valentina Ortiz Bustos

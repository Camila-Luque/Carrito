# CamSchool 🛒✏️

Carrito de compras de útiles escolares. Next.js 16 (App Router) + TypeScript + Tailwind 4.
Lógica del carrito probada con Vitest y mutation testing con StrykerJS.

## Correr en local
```bash
npm install
npm run dev
```
Abre http://localhost:3000

## Scripts
| Comando             | Qué hace                                  |
|---------------------|-------------------------------------------|
| `npm run dev`       | Servidor de desarrollo                    |
| `npm run build`     | Build de producción                       |
| `npm run test`      | Pruebas unitarias (Vitest)                |
| `npm run coverage`  | Pruebas + cobertura                       |
| `npm run mutation`  | Mutation testing (StrykerJS)              |

## Estructura
```
src/
  app/            páginas (/ y /cart) + layout + globals.css
  components/     Navbar, Item, ItemList, CartContext
  lib/
    cart.ts       <- LÓGICA PURA (lo que StrykerJS muta y Vitest prueba)
    cart.test.ts  <- pruebas unitarias
    products.ts   <- los 5 productos
public/images/    imágenes de los productos
```

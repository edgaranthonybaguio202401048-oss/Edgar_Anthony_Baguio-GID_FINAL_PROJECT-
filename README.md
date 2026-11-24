# PineBrew Cafe Iligan – Order App (working prototype)

UX Design project by Edgar Anthony Baguio, Block B.

Open `index.html` in any browser (Chrome works best). Keep the `photos` folder next to it.

## How the code is organized (all in index.html)
- **`<style>`** – colors, fonts and the look of every screen (cards, buttons, cart bar, nav).
- **ART / PHOTOS** – drawn icons and the 18 coffee photos.
- **DATA** – `MENU` (18 drinks, prices, options), categories, sizes, sugar levels, pickup time slots,
  Iligan barangay delivery fees (`AREAS`) and promo codes (`PROMOS`, e.g. ILIGAN10).
- **STATE** – `S` holds the current screen, cart, pickup/delivery choice, payment method and orders.
  Helper functions compute subtotal, discount, delivery fee and total.
- **Actions** – `addToCart`, `changeQty`, `applyPromo`, `validate` (name, mobile number, address, card)
  and `placeOrder` (processing → order received → status tracker).
- **VIEWS** – one function per screen: `vSplash`, `vMenu`, `vProduct`, `vCart`, `vCheckout`,
  `vProcessing`, `vSuccess`, `vOrders`, `vContact`. `render()` draws the current screen.

This is a class prototype: no real payment is charged and no order is sent to a cafe.

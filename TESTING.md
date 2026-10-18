# TESTING.md — Verification & Testing Guide

## Automated Verification Commands
1. **Type Check & Lint**:
   ```bash
   npm run lint
   # Executes: tsc --noEmit
   ```
2. **Production Build & Bundle**:
   ```bash
   npm run build
   # Executes: node scripts/ensure-icons.cjs && vite build && esbuild server.ts --bundle --platform=node --format=cjs --external:vite --sourcemap --outfile=dist/server.cjs
   ```
3. **Applet Compilation Check**:
   - Use the `compile_applet` tool to verify the entire build pipeline.
   - Use the `lint_applet` tool to verify TypeScript types.

## Manual Verification Procedures
- **Multi-Vertical Switching**: Go to Settings or click the header vertical selector to switch between Restaurant, Kirana, Medical, etc. Verify that the Restaurant tab appears when Restaurant vertical is active.
- **Restaurant Table Management**: Go to the Tables view, verify 6 default tables (`T-1` to `T-6`), add/edit tables, and click "Take Order" to populate POS with table number.
- **Invoicing & Thermal Printing**: Create sales/purchase invoices, test UPI QR code generation, thermal slip preview, and PDF/print export.

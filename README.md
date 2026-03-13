## Error Type
Build Error

## Error Message
Module not found: Can't resolve '../messages/' <dynamic> '.json'

## Build Output
./src/i18n/request.ts:14:22
Module not found: Can't resolve '../messages/' <dynamic> '.json'
  12 |   return {
  13 |     locale,
> 14 |     messages: (await import(`../messages/${locale}.json`)).default,
     |                      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  15 |   }
  16 | })
  17 |

Import trace:
  Server Component:
    ./src/i18n/request.ts
    ./node_modules/next-intl/dist/esm/development/server/react-server/getConfig.js
    ./node_modules/next-intl/dist/esm/development/server/react-server/getLocale.js
    ./src/app/layout.tsx

https://nextjs.org/docs/messages/module-not-found

Next.js version: 16.1.6 (Turbopack)

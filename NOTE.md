# path to download the pocketbase database

https://pocketbase.io/

# to generate the admin ui

./pocketbase.exe serve

# outcome of above execution

PS E:\Code\nextjs\nextjs13-todolist> ./pocketbase.exe serve

> Server started at: http://127.0.0.1:8090

- REST API: http://127.0.0.1:8090/api/
- Admin UI: http://127.0.0.1:8090/_/

# update nextjs.config.js to support the new feature use app folder instead of pages folder for file system routing

/\*_ @type {import('next').NextConfig} _/
const nextConfig = {
reactStrictMode: true,
swcMinify: true,
experimental: { appDir: true },
};

module.exports = nextConfig;

# update the package file to enable turbo mode

"scripts": {
"dev": "next dev --turbo",
"build": "next build",
"start": "next start",
"lint": "next lint"
},

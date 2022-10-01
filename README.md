# React-Admin

Practicing how to create React-Admin

# Requirements

- [json-server](https://github.com/typicode/json-server)
- [Material UI](https://mui.com/)

# How to use

## Install Json-Server

1. Init npm package `npm init -y`
2. Install Json-Server `npm i json-server`
3. Add script to run server `"server": "json-server --watch db.json --port 5000"`
4. Create `db.json` file and simple 'json' database
5. Run the server `npm run server` and test it
6. Create React app called `client` using `npx create-react-app client`
7. Add proxy on React `client` package.json, `"proxy": "http://localhost:5000"`
8. Add script to run client `"client": "npm start --prefix client"`, and test it by running `npm run client`.
9. Try to run the both server and client by install `npm i concurrently` and add it in the script `"dev": "concurrently \"npm run server\" \"npm run client\""`, then run `npm run dev`
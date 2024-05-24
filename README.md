# `Roger's Sign In using Internet Identity Azle Project`

Welcome to  `roger_sign_in_azle` project and to the Internet Computer development community.

To get started, you might want to explore the project directory structure and the default configuration file. Working with this project in your development environment will not affect any production deployment or identity tokens.

If you want to start working on your project right away, you might want to try the following commands:

```bash
cd roger_sign_in_azle/
npm install

```

### Note Running th project 
```bash
Make sure That the following are installed in your system 
#1. 
apt install pkg-config

#2. 
apt install rust 

#3. 
apt-get install podman
```

## Running the project locally

If you want to test your project locally, you can use the following commands:

```bash
# Starts the replica, running in the background
dfx start --background
# Insall all dependencies 
npm install
# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Once the job completes, your application will be available at `http://localhost:4943?canisterId={asset_canister_id}`.

If you have made changes to your backend canister, you can generate a new candid interface with

```bash
npm run generate
```

at any time. This is recommended before starting the frontend development server, and will be run automatically any time you run `dfx deploy`.

If you are making frontend changes, you can start a development server with

```bash
npm start
```

Which will start a server at `http://localhost:8080`, proxying API requests to the replica at port 4943.
